```mermaid
    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorNaInternet
    SensoresAparelho --|> iPhone

    class SensoresAparelho {
        <<interface>>
        #deslizarParaCima()
        #deslizarParaBaixo()
        #deslizarParaEsquerda()
        #deslizarParaDireita()
        #desligarTela()
        #ligarTela()
        #virarTela()
        #alterarVolume()
    }

    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
        +selecionarFilme(String filme)
        +selecionarVideoClipe(String video)
        +atribuirNota(number nota)
        +verAlbuns()
    }

    class AparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
        +sincronizarContantos()
        +salvarFavorito(String numero)
        +enviarMensagem(String numero, String mensagem)
        +abrirAlbumFotos()
    }

    class NavegadorNaInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +removerAba(number abaId)
        +atualizarPagina()
        +verClima()
        +verAcoes()
        +abrirMapas()
        +abrirEmail()
    }

```