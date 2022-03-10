# story_telling_creator

Esse é um projeto para a criação de uma interface gráfica para a criação de histórias com escolhas que serão codificadas em json.


A estrutura do json que irá guardar a história será a seguinte:

```
{"Escolhas": [
    {
        "id": 1,
        "História": "Acabou a comida da sua geladeira, você sai as 21:00 da noite para buscar comida no mercado (2 quarteirões da sua casa)...",
        "Opções": [
            {"Id": 1, "Texto": "Ir de carro", "link": 2},
            {"Id": 2, "Texto": "Ir a pé", "link": 3}
        ]
    },

    {
        "id": 2,
        "História": "Você está indo de carro, mas uma pessoa de parou e pediu carona, ela falou que está indo para o mesmo supermercado.",
        "Opções": [
            {"Id": 1, "Texto": "Dar a carona", "link": null},
            {"Id": 2, "Texto": "Não dar carona", "link": null}
        ]
    },

    {
        "id": 3,
        "História": "Você chegou ao supermercado, houviu alguns barulhos estranhos ao longo do caminho, perto de casa. Está com medo...",
        "Opções": [
            {"Id": 1, "Texto": "Voltar para casa e tentar dormir", "link": null},
            {"Id": 2, "Texto": "Ir para a casa de amigos", "link": null}
        ]
    }
]}

```

As escolhas são colocadas num array, onde cada escolha tem uma história, que é a história prévia à própria escolha, as opções de escolha e cada opção de escolha tem um link para uma nova escolha.
