**Regiões**  
        - Estão distribuídas globalmente.  
        - Uma região é um *cluster* de data centers.  
        - A maioria dos serviços possui escopo regional, ou seja, estão vinculados a uma região específica para garantir melhor disponibilidade.  

**Zonas de Disponibilidade (AZs)**  
        - Cada região possui no mínimo 3 e no máximo 6 zonas de disponibilidade.  
            - Exemplo: `ap-southeast-2a`, `ap-southeast-2b`, `ap-southeast-2c`.  
        - Uma AZ é composta por um ou mais data centers.  
        - As AZs são separadas fisicamente e isoladas para evitar desastres em cascata.  
            - Exemplo: Uma enchente em uma AZ não afeta as outras.  
        - Conectadas por redes de alta largura de banda e baixa latência.  

**Pontos de Presença (Edge Locations)**  
        - Mais de 400 pontos de presença (Edge Locations) e 10+ caches regionais.  
        - Distribuídos em mais de 90 cidades em 40+ países.  

**Serviços Globais**  
        - Identity and Access Management (IAM).  
        - Route 53 (Serviço de DNS).  
        - CloudFront (Rede de Distribuição de Conteúdo).  
        - WAF (Web Application Firewall).  

**Serviços com Escopo Regional**  
        - Amazon EC2 (Infraestrutura como Serviço).  
        - Elastic Beanstalk (Plataforma como Serviço).  
        - Lambda (Função como Serviço).  
        - Rekognition (Software como Serviço).  

Para mais informações:  
        [AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services)
