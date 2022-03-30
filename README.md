<table cellspacing="0" cellpadding="0">
    <tr>
        <td><img src="https://user-images.githubusercontent.com/8747446/160939167-1e70640f-ba7d-48fa-93a3-7167520fbbd7.png" width="300"></td>
        <td><img src="https://user-images.githubusercontent.com/8747446/160938749-10b34fed-c9e8-4644-8218-2d61fcae5299.png" width="400"></td>
    </tr>
</table>

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

Or via command line via `rasa shell`, see ![example](https://github.com/CrossLangNV/C4C_rasa/tree/main/media/C4C_2.png?raw=true)
