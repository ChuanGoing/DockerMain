FROM microsoft/dotnet:2.2-aspnetcore-runtime AS base
MAINTAINER CHUANGOING
WORKDIR /app
EXPOSE 5000

FROM microsoft/dotnet:2.2-sdk AS publish
WORKDIR /src
COPY . .
RUN dotnet restore
WORKDIR "/src/ChuanGoing.WebOnline"
RUN dotnet publish "ChuanGoing.WebOnline.csproj" -c Release -o /app

FROM base AS final
WORKDIR /app
COPY --from=publish /app .
CMD ["dotnet", "ChuanGoing.WebOnline.dll"]
