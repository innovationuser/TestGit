Inlux Launch Steps -
URL : http://localhost:8086
Go to CMD and execute influd.exe and then influx.exe

Grafana Launch Steps -
URL : http://localhost:8081
Id - admin
Pass - qwerty@321


Curl commands to publish to influx
For inserting : C:\>curl -i -XPOST "http://localhost:8086/write?db=demo" --data-binary @\GIT\TestGit\Publish.txt
For quering the DB :C:\>curl -G "http://localhost:8086/query?pretty=true" --data-urlencode "db=demo" --data-urlencode "q=SELECT * FROM Application_Dependency_Tracking"