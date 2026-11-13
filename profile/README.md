# Sunrise Initiative

Desenvolvemos o **Sunrise OS**, um sistema desktop de código aberto sobre Linux para PCs x86-64 com UEFI. A interface combina transparências e referências ao estilo Frutiger Aero, com uma variante em violeta e laranja chamada **Sunrise Glass**.

## Onde estamos

O primeiro protótipo do menu de aplicativos já abre em uma sessão Wayland no Fedora e lista os aplicativos instalados. O catálogo em Rust passou nos testes iniciais. A abertura dos aplicativos pela interface e o teste em uma segunda VM ainda estão pendentes.

O próximo marco é uma sessão de desenvolvimento com painel, dock e menu de aplicativos, acompanhada de uma prova separada do compositor em uma sessão Wayland aninhada.

## Como o desktop é construído

| Componente | Tecnologia e papel |
| --- | --- |
| Shell | Qt 6 e QML para painel, dock e menu de aplicativos |
| Lógica do sistema | Rust para descobrir e abrir aplicativos e integrar serviços |
| Compositor próprio | Rust e Smithay, com a primeira prova prevista em modo aninhado |
| Ambiente de desenvolvimento | Fedora em VM, com UEFI e Wayland |

## Primeira prévia pública

A meta é disponibilizar um desktop funcional em máquina virtual com três aplicativos próprios: **Sunrise Files**, **Calculadora** e **Bloco de Notas**. O **Sunrise Launcher** está planejado como a loja oficial para instalar e atualizar aplicativos e acompanhar novas versões do sistema.
