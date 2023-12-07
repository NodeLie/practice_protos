# practice_protos
#Для использования необходимо:
<p>Для начала, вам её нужно установить, подробности по установке [тут](https://grpc.io/docs/languages/go/quickstart/). Внимательно читайте инструкцию — нужно установить не только утилиту, но и плагин для Go.</p> <br>
Установка для Windows и если установлен Go: </br>
<ul>
    <li>go install go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2</li>
    <li>protoc-gen-go-grpc --version</li>
    <li>go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28</li>
    <li>protoc-gen-go --version</li>
    <li>go install github.com/go-task/task/v3/cmd/task@latest</li>
</ul>
<p>Если не хотим использовать Taskfile команда для генерации:</p>
   <b>protoc -I proto proto/sso/sso.proto --go_out=./gen/go/ --go_opt=paths=source_relative --go-grpc_out=./gen/go/ --go-grpc_opt=paths=source_relative</b> 
