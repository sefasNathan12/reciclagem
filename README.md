# Spot Trash
projeto web (v3) que ajuda pessoas a descobrir **onde e como entregar materiais para reciclagem** (plástico, papel, vidro, metal, óleo de cozinha, orgânicos, pilhas e eletrônicos). Projeto Integrador – Design Profissional (Turma B), desenvolvido por Sávio Nathannael Batista Galdino e Sefas Nathan Batista Galdino.

> **Aviso:** é um protótipo para teste exploratório. Cidades, pontos de coleta, endereços e horários são **exemplos inventados** e não representam estabelecimentos reais. Confirme sempre com o ponto antes de ir.

## Problema

No Brasil, a Política Nacional de Resíduos Sólidos (Lei nº 12.305/2010) prevê coleta seletiva e logística reversa, e o Decreto nº 10.240/2020 trata dos eletroeletrônicos de uso doméstico. Mesmo assim, a coleta seletiva ainda não cobre todos os bairros e boa parte do que poderia ser reciclado se perde (dados da ABRELPE, a conferir na edição mais recente). O Spot Trash tenta reduzir a barreira de informação: onde entregar cada material e como se preparar. Ele **não coleta nem recicla** nada. **[CONFIRMAR: números atualizados do Panorama ABRELPE]**

## O que o protótipo faz

- **Início:** busca por cidade, bairro e tipo de material (11 categorias: celulares, pilhas e baterias, computadores, eletrodomésticos pequenos, cabos, plástico, papel e papelão, vidro, metal, óleo de cozinha usado e orgânicos).
- **Alternativas ao descarte:** reduzir e reutilizar, consertar, doar ou trocar, antes da lista de pontos.
- **Pontos:** lista os pontos que aceitam o aparelho escolhido e indica se estão abertos agora.
- **Detalhe do ponto:** endereço, horário, tipos aceitos e a data da última verificação.
- **Antes de entregar:** passo a passo de preparo por material; para eletrônicos, inclui aviso de segurança sobre baterias estufadas. Para os demais, lembra de confirmar as regras locais.
- **Que material é este?:** guia para identificar a categoria do item (por exemplo, garrafa PET, caixa de papelão, lata, óleo de cozinha).
- **Informar mudança:** formulário para avisar que um ponto mudou, com verificação para impedir que dados pessoais (como CPF, e-mail ou telefone) sejam enviados.
- **Quero ser um ponto de coleta:** cadastro de um novo ponto, com opção de apagar o cadastro.
- **Ajustes de leitura:** aumentar ou diminuir o texto e alternar o tema claro e escuro.

## Privacidade

- Não há login, cadastro de usuário nem coleta de dados pessoais.
- Pontos cadastrados, relatos e preferências ficam salvos **somente no navegador do aparelho** (`localStorage`). Nada é enviado a um servidor.
- Nenhuma requisição de rede é feita pelo código do protótipo (fora o carregamento das fontes do Google Fonts).

## Acessibilidade

Medidas adotadas no protótipo:

- HTML semântico, rótulos nos controles e papéis ARIA em elementos dinâmicos;
- navegação por teclado com foco visível;
- ajuste do tamanho do texto e tema claro e escuro (respeita a preferência do sistema);
- layout responsivo para celular e computador e respeito à preferência por menos movimento.

**Importante:** a meta do projeto é seguir as WCAG 2.2 nível AA, mas **a conformidade não foi auditada formalmente**. **[CONFIRMAR: nota do Lighthouse e resultado do teste com leitor de tela, se feitos]**

## Como executar

O protótipo é estático. Basta baixar os arquivos e abrir `index.html` em um navegador. Não há dependências nem etapa de build.

```
index.html   estrutura da página
style.css    estilos (tema claro e escuro, layout responsivo)
script.js    telas, regras e armazenamento local
```


