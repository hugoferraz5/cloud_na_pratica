# Projeto de Cloud - Migração de toda aplicação e dados para um ambiente MultiCLoud.

<div align="center">
<img src="https://github.com/user-attachments/assets/79c55430-1284-4de6-ae8d-278515a5dcf3" width="700px" />
</div>

# Questão de negócio

Durante a pandemia, uma rede de hotéis e resorts de luxo, que anteriormente recebia seus hóspedes sem a necessidade de testes de saúde, enfrentou a necessidade de adotar novas medidas para garantir a segurança de seus clientes e funcionários. Passou-se a exigir testes de Covid-19 realizados algumas horas antes do check-in, como requisito para o acesso a todos os setores da rede.

No entanto, à medida que a demanda aumentava, o data center local, utilizado para gerenciar as operações, mostrou-se incapaz de suportar o crescimento. Isso resultou em lentidão no sistema, comprometendo a experiência dos hóspedes e atrasando processos como o check-in.

Diante dessa situação, a rede tomou a decisão estratégica de migrar todas as aplicações e dados para a nuvem, buscando escalabilidade, desempenho aprimorado e continuidade operacional para atender à crescente demanda de forma eficiente.

# Solução

Para resolver o problema mencionado, a rede de hotéis implementou rapidamente a migração de todas as suas aplicações e dados para a nuvem. Essa solução foi adotada com urgência devido à alta demanda e à necessidade de garantir a continuidade das operações, sem interrupções nas atividades. O processo exigiu conhecimento técnico especializado e uma execução ágil para atender às expectativas e manter a qualidade do serviço oferecido aos hóspedes. 

Para isso, o gerente de TI contratou uma consultoria para a realização dessas atividades utilizando o Google Cloud como servidor principal devido a rede ja possuir serviços rodando por la.

Entre os serviços disponíveis na nuvem, foi criada uma rede VPC para gerenciar toda a comunicação interna no Google Cloud. Além disso, o Google Container Registry foi utilizado para armazenar a imagem da aplicação, que foi modernizada ao migrar de uma máquina virtual para um contêiner. O armazenamento de dados da rede foi feito no Google Cloud SQL, enquanto a orquestração dos contêineres e a comunicação com o banco de dados foram gerenciadas pelo Google Kubernetes Engine (GKE). Essa abordagem automatizou o ambiente, tornando-o mais escalável e flexível, atendendo às necessidades de alta demanda e garantindo eficiência operacional.

Além disso, foi utilizado o AWS S3 para o armazenamento dos resultados dos exames de Covid-19 dos hóspedes em formato PDF. Essa escolha foi estratégica, pois o S3 já era utilizado para backups, o que ajudou a reduzir custos operacionais.

Por fim, para garantir agilidade e automação no provisionamento, toda a arquitetura foi criada utilizando o Terraform, uma ferramenta de infraestrutura como código. Com essa abordagem, a solução foi implementada com sucesso, atendendo às demandas de forma eficiente e moderna.

<div align="center">
<img src="https://github.com/user-attachments/assets/7036a6a4-43fe-46d6-b696-d4403e930d11" width="700px" />
</div>

<div align="center">
<img src="https://github.com/user-attachments/assets/a2ce940b-81dc-410a-b841-9915966439d8" width="900px" />
</div>



