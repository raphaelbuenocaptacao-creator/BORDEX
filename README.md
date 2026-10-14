# BORDEX — Central de Notas Fiscais

Aplicativo estático para uso interno na conferência e preparação de notas fiscais e borderôs de profissionais.

## Recursos da primeira versão
- Cadastro, edição, exclusão e busca de profissionais.
- Importação de CSV UTF-8 (modelo disponível no próprio aplicativo).
- Comissão, fixo, mínimo garantido, SPIFF, ajuda de custo, descontos e faltas.
- Regra padrão: descontos exclusivamente na comissão; exceção para mínimo precisa ser explicitamente autorizada.
- Faltas registradas separadamente; escolha manual de qual nota recebe o abatimento.
- Comparação do total calculado com o total oficial da planilha; avisos de divergências.
- Duas notas fiscais separadas e mensagem completa copiável.
- Aprovação interna, navegação próximo/anterior e observações.
- Exportação CSV e backup/restauração JSON.
- Datas de competência editáveis (inicialmente setembro/2026 e novembro/2026).

## Abrir e publicar
O aplicativo está em `index.html`. Abra-o no navegador ou publique o repositório pelo GitHub Pages em Settings > Pages > Deploy from a branch > main > /(root) > Save.

O repositório é **público**: **não adicione planilhas ou dados de profissionais como arquivos Git**. Os registros ficam no armazenamento local do navegador e não são sincronizados entre aparelhos. Faça backup frequente e não compartilhe o navegador com terceiros. Não há autenticação no MVP.

## Regras de segurança operacional
O sistema **não emite NFS-e**, não envia notas automaticamente, não realiza pagamentos e não valida legislação tributária. "Aprovado" significa apenas controle interno. Divisão de faltas por nota, descontos em mínimos e divergências exigem decisão explícita do gestor.

## Próximas fases
Autenticação individual, PostgreSQL com RLS, histórico e auditoria persistentes, integração XLSX nativa, permissões e implantação em domínio protegido.