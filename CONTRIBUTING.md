# Contribuir com o Sunrise

O Sunrise desenvolve aplicativos desktop abertos para criação e produtividade. O site apresenta o planejamento e o launcher reúne o catálogo e vínculos locais.

## Relatar problemas

Abra uma issue no repositório afetado. Inclua versão ou commit, sistema operacional, passos para reproduzir, resultado esperado e resultado observado. Imagens ajudam a descrever falhas visuais. Remova informações pessoais dos anexos.

## Propor mudanças

Descreva a necessidade do usuário e o escopo. Em mudanças de arquitetura, formato de arquivo ou segurança, registre a proposta para discussão antes de ampliar a implementação.

## Enviar código

Crie uma branch a partir de main e abra um pull request com resumo da mudança e verificações executadas. Use mensagens de commit no padrão Conventional Commits, como feat, fix, docs ou ci.

No launcher, execute cargo fmt --check, cargo test --locked e cargo clippy --locked --all-targets --all-features -- -D warnings dentro da pasta do projeto. No website, instale com npm ci e valide com npm run build. Os READMEs dos produtos detalham o ambiente.

Preserve acessibilidade, funcionamento offline e preferências existentes. Nos ajustes de UI, confira os temas claro e escuro, janela compacta, teclado e redução de movimento.

## Código e recursos de terceiros

O código próprio do launcher usa GPL-3.0-only. Confira a licença do repositório e preserve atribuições de dependências e recursos. Implemente a partir dos requisitos Sunrise e de referências permitidas, registrando procedência e limites das verificações.

Mantenha as discussões respeitosas, concretas e voltadas ao problema.
