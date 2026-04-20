
# Política de Segurança

A segurança dos dados e da infraestrutura do Élen é levada a sério. Este documento explica como relatar vulnerabilidades e o que esperar do nosso processo.

## Versões suportadas

Atualmente, apenas a versão mais recente do código disponível no branch `main` recebe atualizações de segurança. Correções não são aplicadas retroativamente a versões antigas ou forks.

| Versão | Suporte           |
|--------|-------------------|
| main   | Sim               |
| < 1.0  | Não               |

## Como relatar uma vulnerabilidade

Se você descobrir uma falha de segurança (por exemplo, exposição acidental de chaves, injeção de código, problemas de autenticação), **não abra uma issue pública**.

Em vez disso, envie um e-mail para:

**contato.luiz404@gmail.com**

Inclua no e-mail:

- Uma descrição clara do problema.
- Passos para reproduzir a vulnerabilidade.
- Possível impacto (exemplo: vazamento de dados, execução de código).
- Sugestão de correção, se houver.

Responderemos em até **72 horas** para confirmar o recebimento.

## Processo de tratamento

1. **Confirmação**: você receberá uma resposta inicial em até três dias úteis.
2. **Análise**: nossa equipe investigará o relatório e poderá pedir informações adicionais.
3. **Correção**: uma vez validada, a correção será desenvolvida em um branch privado.
4. **Divulgação**: após a correção ser implantada, publicaremos um aviso de segurança (se necessário) e creditaremos você, caso deseje.

## Práticas de segurança do projeto

- As chaves de API do Supabase usadas no front-end são apenas a chave `anon`, que tem permissões limitadas e seguras por Row Level Security.
- O código não armazena dados de usuários ou arquivos enviados.
- O deploy é feito via Vercel com HTTPS obrigatório.

## Recompensas

No momento, não oferecemos recompensas financeiras. No entanto, seu nome será incluído nos créditos de segurança (se autorizado) e terá nosso sincero agradecimento.

## O que não é considerado vulnerabilidade

- Problemas já conhecidos e listados em issues públicas.
- Configurações incorretas em ambientes locais que não afetam a versão em produção.
- Ausência de funcionalidades que não comprometem a segurança dos dados.

Agradecemos por ajudar a manter o Élen seguro para todos.
