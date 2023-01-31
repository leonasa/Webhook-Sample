#See https://aka.ms/containerfastmode to understand how Visual Studio uses this Dockerfile to build your images for faster debugging.

FROM mcr.microsoft.com/dotnet/aspnet:7.0 AS base
WORKDIR /app
EXPOSE 80
EXPOSE 443

FROM mcr.microsoft.com/dotnet/sdk:7.0 AS build
WORKDIR /src
COPY ["Webhook2Kafka/Webhook2Kafka.csproj", "Webhook2Kafka/"]
RUN dotnet restore "Webhook2Kafka/Webhook2Kafka.csproj"
COPY . .
WORKDIR "/src/Webhook2Kafka"
RUN dotnet build "Webhook2Kafka.csproj" -c Release -o /app/build

FROM build AS publish
RUN dotnet publish "Webhook2Kafka.csproj" -c Release -o /app/publish /p:UseAppHost=false

FROM base AS final
WORKDIR /app
COPY --from=publish /app/publish .
ENTRYPOINT ["dotnet", "Webhook2Kafka.dll"]