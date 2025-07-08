# Estrutura de uma Política IAM

## Version (Versão)
- Indica a versão da linguagem da política.
- Deve sempre incluir `"2012-10-17"`.

## Id (Identificador)
- Um identificador para a política.
- É opcional.

## Statement (Declaração)
- Contém uma ou mais declarações individuais.
- É um campo obrigatório.

As declarações consistem em:

- **Sid (Identificador da Declaração):**
    - Um identificador para a declaração. É opcional.
- **Effect (Efeito):**
    - Define se a declaração permite (`Allow`) ou nega (`Deny`) o acesso.
- **Principal (Principal):**
    - A conta, usuário ou função à qual esta política se aplica.
- **Action (Ação):**
    - Uma lista de ações que esta política permite ou nega.
- **Resource (Recurso):**
    - Uma lista de recursos aos quais as ações se aplicam.
    - **Condition (Condição):** Condições para quando esta política está em efeito.

---

## Exemplo de uma política IAM em JSON

```json
{
    "Version": "2012-10-17",
    "Id": "MinhaPoliticaDeExemplo",
    "Statement": [
        {
            "Sid": "PermitirAcessoEC2ELBCloudWatch",
            "Effect": "Allow",
            "Action": [
                "ec2:Describe*",
                "elasticloadbalancing:Describe*",
                "cloudwatch:ListMetrics",
                "cloudwatch:GetMetricStatistics",
                "cloudwatch:Describe*"
            ],
            "Resource": "*"
        }
    ]
}
```
