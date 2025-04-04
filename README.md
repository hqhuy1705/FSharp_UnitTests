# FSharp_UnitTests_Exam

###### Go to the Tests project
```
cd OrderProcessing.Tests
```

###### Execute test with coverage enable
```
dotnet test /p:CollectCoverage=true /p:CoverletOutput=./coverage/ /p:CoverletOutputFormat=cobertura
```

###### Install ReportGenerator
```
dotnet tool install --global dotnet-reportgenerator-globaltool
```

###### Generate the Report
```
~/.dotnet/tools/reportgenerator -reports:"./coverage/coverage.cobertura.xml" -targetdir:"./coverage-report" -reporttypes:Html
```
