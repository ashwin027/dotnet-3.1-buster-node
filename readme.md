## .Net 3.1 docker image with nodejs (12.1)
The current .Net 3.1 docker image does not include node js, and building SPAs with a JavaScript framework as part of the .Net project is currently not supported out of the box. The image in this repository includes nodejs and can be used in place of the Microsft provided image to build SPAs. To use it, simply replace this line in your dotnet project docker file,

`FROM mcr.microsoft.com/dotnet/core/sdk:3.1-buster AS build`

with

`FROM ashwin027/dotnet-3.1-buster-node:latest AS build`

Enjoy!
