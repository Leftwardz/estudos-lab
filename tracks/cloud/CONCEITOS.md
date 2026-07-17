# Conceitos — Cloud

## Modelos de serviço

| Modelo | Você gerencia | Provedor gerencia | Exemplo |
|--------|---------------|-------------------|---------|
| IaaS | SO, runtime, app | Hardware, rede | EC2, Compute Engine |
| PaaS | App, dados | Runtime, SO, HW | Heroku, App Engine |
| SaaS | Uso | Tudo | Gmail, Notion |

## Responsabilidade compartilhada

- **Cliente:** dados, configuração, patches de SO (em IaaS), IAM
- **Provedor:** hardware, rede física, hypervisor, serviços gerenciados

## Object Storage

```
s3://bucket-name/path/to/object.jpg
```

- Durabilidade alta (11 nines no S3)
- Versionamento e lifecycle policies
- Acesso via IAM ou URLs assinadas

## Serverless

- Escala automática por request
- Paga por execução (não por servidor ligado)
- Cold start em funções pequenas
- Ideal para: APIs leves, processamento de eventos, cron

## VPC (rede virtual)

```
VPC 10.0.0.0/16
├── Subnet pública  10.0.1.0/24  (internet gateway)
└── Subnet privada  10.0.2.0/24  (sem acesso direto à internet)
```

## IAM — princípio do menor privilégio

```json
{
  "Effect": "Allow",
  "Action": ["s3:GetObject"],
  "Resource": "arn:aws:s3:::meu-bucket/*"
}
```

## Well-Architected (5 pilares)

1. Excelência operacional
2. Segurança
3. Confiabilidade
4. Eficiência de performance
5. Otimização de custos
