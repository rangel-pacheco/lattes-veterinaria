# Skill lattes-veterinaria: onde cadastrar no Lattes

Ajuda docentes a identificar **onde registrar produções e atividades no Lattes**, quais comprovantes reunir e como analisar o enquadramento na APCN de **Medicina Veterinária — Área 24 da CAPES**.

Baseada no Orientador APCN 2026 e na Ficha de Avaliação 2025–2028, com distinção entre cursos acadêmicos e profissionais.

## Instalação rápida no Codex

No Codex com suporte a skills, peça:

```text
$skill-installer
Instale a skill deste diretório do GitHub:
https://github.com/rangel-pacheco/lattes-veterinaria/tree/main/lattes-veterinaria
Após a instalação, verifique se aparece como $lattes-veterinaria.
```

A instalação copia arquivos; **não cria sincronização contínua** com o GitHub. O nome para invocar a skill é `$lattes-veterinaria`. Se não aparecer, reinicie o Codex e confira a instalação.

### Alternativa: instalação manual

Baixe o ZIP em **Code → Download ZIP**, extraia e copie somente a pasta `lattes-veterinaria`, contendo `SKILL.md` e `references/`:

| Sistema | Diretório |
|---|---|
| Windows | `%USERPROFILE%\\.agents\\skills\\` |
| macOS/Linux | `~/.agents/skills/` |

A instalação em Claude Code pode seguir o mecanismo de skills compatível do aplicativo (por exemplo, pasta `~/.claude/skills/`); isso **não garante acesso ao navegador nem ao Lattes**. No ChatGPT, a disponibilidade de instalação de skills depende do ambiente e do plano.

### Atualizar a skill instalada

Peça ao Codex: `Compare minha skill lattes-veterinaria instalada com a versão mais recente do repositório GitHub. Mostre as diferenças e peça minha confirmação antes de atualizar os arquivos locais, preservando eventuais personalizações.`

**Atenção:** isso é uma verificação sob demanda, não atualização automática em segundo plano. Antes de aplicar atualizações, revise as mudanças do repositório.

## Como usar

Anexe o material, cole um link ou descreva a atividade. Informe **ano, autoria e seu papel, público, projeto/linha e modalidade da proposta**.

Exemplos:

- “Onde cadastro esta cartilha de biossegurança no Lattes?”
- “Ministrei uma oficina de 12 horas. Como registrar? Ela se enquadra como PTT?”
- “Elaborei um protocolo sanitário adotado por uma cooperativa. Como comprovar?”
- “Organizei um evento virtual. Qual o enquadramento na Área 24?”
- “Revise minhas produções para selecionar os destaques da APCN.”

A resposta indica **cadastro provável, enquadramento, documentos comprobatórios e pendências**, com identificação das fontes. Você também pode usar o [modelo de portfólio](PORTFOLIO.md).

## Cadastro assistido no Lattes (opcional)

Com um Codex que disponibilize navegação no navegador, o pesquisador pode solicitar:

```text
$lattes-veterinaria
Quero cadastrar as produções dos documentos que vou anexar.
Primeiro verifique possíveis duplicidades, classifique cada item
e mostre um plano de cadastro para minha aprovação.
Se houver ferramentas de navegação adequadas e uso permitido,
abra a Plataforma Lattes oficial para que eu faça o login pessoalmente.
Após minha autorização, preencha e salve os registros aprovados,
conferindo cada salvamento. NÃO envie o currículo para publicação.
Ao final, apresente um relatório do que foi realmente salvo,
do que já existia e das pendências.
```

O agente pode preencher formulários quando dispõe de ferramentas apropriadas e de autorização. **A skill em si não acessa sites nem é uma integração do CNPq.** A execução depende das condições de uso da Plataforma Lattes, das ferramentas disponíveis e da validação do pesquisador. Não compartilhe senha, código de autenticação ou token com a IA. O envio do currículo ao CNPq é sempre feito **exclusivamente pelo titular**.

Consulte o [protocolo de cadastro assistido](lattes-veterinaria/references/protocolo-cadastro-assistido.md), que descreve autorização, análise de duplicidades, conferência, auditoria e condições para interromper a execução.

## O que diferencia esta skill

- **[APCN-2026]** Considera os dez grupos de PTT da Veterinária e seus valores de referência para propostas profissionais.
- **[APCN-2026]** Cursos de formação profissional exigem **pelo menos 16 horas**; eventos virtuais têm valor próprio.
- **[APCN-2026]** Orienta a seleção de até cinco produções por docente nos cinco anos anteriores à submissão, conforme o edital.
- **[Ficha-2025-2028]** Separa avaliação quadrienal da pontuação de entrada na APCN.
- **[Inferência]** Diferencia atividade e produto, evita duplicidade e aponta caminhos de cadastro que precisam ser confirmados na interface do Lattes.

As tabelas e explicações completas ficam nas [referências da skill](lattes-veterinaria/references), mantendo esta página como guia de início rápido.

## Limites

A skill, sozinha, **não acessa nem edita seu Lattes**. Em um agente com navegação autorizada, pode orientar o preenchimento e a gravação de registros; isso não constitui integração oficial do CNPq. A ferramenta não envia dados à Sucupira e não garante pontuação ou aprovação. ISBN, DOI e downloads, isoladamente, não comprovam impacto. A avaliação depende de autoria, período, aderência e evidências. Confirme documentos e edital vigentes antes da submissão.

## Fontes e créditos

[Fontes oficiais da Área 24](lattes-veterinaria/references/fontes-e-vigencia.md): Orientador APCN 2026, Documento de Área e Ficha 2025–2028.

Inspiração na proposta do repositório [jalinegm/lattes-apcn](https://github.com/jalinegm/lattes-apcn), que referencia a Oficina Lattes da Profa. Priscila Tavares. Esta adaptação utiliza critérios próprios da Medicina Veterinária, sem importar regras de outras áreas.

Material independente de apoio. Atualização desta página: **11/11/2026**.
