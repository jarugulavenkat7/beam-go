# beam-go
## Steps to run the beam-go
#### Download and Install
* Download and Install GO from [https://go.dev/doc/install](https://go.dev/doc/install)
#### Check Version
* After Downloading and Installing, Check your GO version using the command  `go version`
#### Create a project and a Repository
* Create a project with name beam-go in your 44517 folder.
* Create a git repo with exactly the same name of your project in local machine i.e beam-go.
* In your folder, run go mod init `github.com/jarugulavenkat7/beam-go`
#### Get the SDK and the examples
* command `go get -u github.com/apache/beam/sdks/v2/go/pkg/beam`
#### Add the input file
* create the sample.txt file and add content from [here](https://00f74ba44bd17d64b0e5795b97f8bb2d35211be6bd-apidata.googleusercontent.com/download/storage/v1/b/apache-beam-samples/o/shakespeare%2Fkinglear.txt?jk=AFshE3UeJ2xt7wKyuu8EYa1DzDNgVKE2yjdBUfcXGj63aIPGsRoyQ8meOvgx22I5JlgGjXdxTvWF6OJEzCmZnC_9dT1zd0k3G8sxa72rqCBaa1YQorm4Rtd-TEyZ1NLcP64pR6BKkGB7wXafjprLYuRp_U7IPPzBVYpy2R8rJeaY4JEZ3cIBhzlzm-Zak1kc54R5PaiO0BphHR6hiE9__U0tmUFAsLpzGQkyJ0OTb4uqQbBHckZp-ybWtXTO9gfZ7QSgjkRBCGq6k36yv-NbK2trEt8l2m-GZm9uCNlOsW0rBWQW4jc_exqM6fgopn23tF3hgUe6Zd1U1zNkR4r0Ws2GhTSrlxh_m7GAFcMxxtPYAu8K3OVZtu6VIm3uoyIfpjyqY4GciJO4wpRgvr1pj1_38lleZRdmU9XlxtUoCMyF3uxKBIYYK7Wy3REyhHfVTe5BvNfutEix3QNUt4_zOrsTVqCtCuOgUxAFylNYclnNh0Jf40s2ZX4koPa46QSlt0nFTMtEfOzIV64Q9TL3cVssTOwO6DenmVvk6hm__JevI7m8L0U_anUa4pPQWzYyckEF5pEpX2UATWim7Z5fBRWW7WcZ2vZTFWdGitxDqOPhLP7vaMalBHG3pp_F1JToF3v6JT_ImZAGKycY9RWQHTFM3ZUa6UfWUqIHCUw6zx9fsFzNAL40EVTP4xOd8XnWbujEQkZbVcprnTo1LzKUUpBfrbVaFv8CV_8aCebDoSOYvKFtLvrvR32MKkWNX_i_8ZtmmjcLo7q005R1ZNILPfs1P482Oyb48k4xWa0MCYeNp-8kSn8NKRoYIZ0eK3nKuJerrvjdWd8RFrShJOAE8nPU-bYcJ3ktwjVyhCsuEKv0QjGI4eiIBQvWYl5InTRgnIwC3wG5Liv0cmteg3yPwPAQloK1yEgt9_392mvPXvjI4uzileHMTKxugYxmzba6Ib-LdzqXk1zfWr5UiP-6H5HWi4s5FKBx&isca=1)
#### Run WordCount
- To get wordcount.go run the command `go install github.com/apache/beam/sdks/v2/go/examples/wordcount`
- If you get an error like "missing go.sum entry for module providing package" then run the command ` go get github.com/apache/beam/sdks/v2/go/pkg/beam/io/filesystem/gcs@v2.37.0`
- To run the wordcount.go use the command `go run wordcount.go --input sample.txt --output counts`
- The output counts file will be generated in the project folder
