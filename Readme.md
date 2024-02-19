# Umbraco Demo

Set up Umbraco site with a local database



    # Ensure we have the latest Umbraco templates
    dotnet new install Umbraco.Templates --force

    # Create solution/project
    dotnet new sln --name "UmbDemo"
    dotnet new umbraco --force -n "UmbDemo" --friendly-name "Administrator" --email "admin@example.com" --password '1234567890' --development-database-type SQLite
    dotnet sln add "UmbDemo"

    dotnet run --project "UmbDemo"
    #Running