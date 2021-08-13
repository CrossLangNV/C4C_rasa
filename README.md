# C4C Rasa

Instructions
------------

use "dbuild.sh" to build the docker image <br />
use "dcli.sh" to start a docker container

Once the docker is up and running type `rasa init` in the command line. 

Next, run `rasa train` to train the chatbot. And `rasa run` to expose a REST endpoint at 5005 port in the localhost.

One can then send a json to `localhost:5005/webhooks/rest/webhook`:


```
{
"sender": "test_user"
"message": "Hello"
}
```

Or via command line via `rasa shell`, see ![swagger](https://github.com/CrossLangNV/C4C_rasa/tree/main/media/C4C_2.png?raw=true)
