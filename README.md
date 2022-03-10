# story_telling_creator

Esse é um projeto para a criação de uma interface gráfica para a criação de histórias com escolhas que serão codificadas em json.


A estrutura do json que irá guardar a história será a seguinte:

```
{
    "Titulo": "Noite aparentemente comum",
    "Escolhas": [
        {
            "id": 0,
            "História": "Acabou a comida da sua geladeira, você sai as 21:00 da noite para buscar comida no mercado (2 quarteirões da sua casa)...",
            "Opções": [
                {"Id": 0, "Texto": "Ir de carro", "link": 1},
                {"Id": 1, "Texto": "Ir a pé", "link": 2}
            ]
        },

        {
            "id": 1,
            "História": "Você está indo de carro, mas uma pessoa de parou e pediu carona, ela falou que está indo para o mesmo supermercado.",
            "Opções": [
                {"Id": 0, "Texto": "Dar a carona", "link": null},
                {"Id": 1, "Texto": "Não dar carona", "link": null}
            ]
        },

        {
            "id": 2,
            "História": "Você chegou ao supermercado, houviu alguns barulhos estranhos ao longo do caminho, perto de casa. Está com medo...",
            "Opções": [
                {"Id": 0, "Texto": "Voltar para casa e tentar dormir", "link": null},
                {"Id": 1, "Texto": "Ir para a casa de amigos", "link": null}
            ]
        }
    ]
}

```

As escolhas são colocadas num array, onde cada escolha tem uma história, que é a história prévia à própria escolha, as opções de escolha e cada opção de escolha tem um link para uma nova escolha.
