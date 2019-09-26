# Installation



## Create database

```powershell
dotnet ef database update -p .\Infrastructure\ -c CatalogContext -s .\Web\ -v
dotnet ef database update -p .\Infrastructure\ -c AppIdentityDbContext -s .\Web\ -v
```

> :bulb: 
>
> 1. `-p`是指DbContext所在工程，通常这个工程是基于`.NET Standard`
> 2. `-s`是指启动工程
> 3. `-c`指应用的DbContext，可以忽略名字空间

 