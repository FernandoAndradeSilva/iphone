classDiagram
direction BT
class AparelhoTelefonico {
<<Interface>>
  + ligar(String) void
  + atender() void
  + iniciarCorreioVoz() void
}
class Iphone {
  + Iphone() 
  + atender() void
  + atualizarPagina() void
  + adicionarNovaAba() void
  + iniciarCorreioVoz() void
  + exibirPagina(String) void
  + pausar() void
  + ligar(String) void
  + selecionarMusica(String) void
  + tocar() void
}
class Main {
  + Main() 
  + main(String[]) void
}
class NavegadorInternet {
<<Interface>>
  + adicionarNovaAba() void
  + atualizarPagina() void
  + exibirPagina(String) void
}
class ReprodutorMusical {
<<Interface>>
  + pausar() void
  + tocar() void
  + selecionarMusica(String) void
}

Iphone  ..>  AparelhoTelefonico 
Iphone  ..>  NavegadorInternet 
Iphone  ..>  ReprodutorMusical 
