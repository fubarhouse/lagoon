# amazee.io Lagoon - where the cool microservices hang out!

The amazee.io lagoon is the amazee.io deployment system, completely independent from any servers running. Perfect for local development, testing new features and taking over the world.

- Schema: [https://www.lucidchart.com/documents/edit/a3cf0c4f-1bc1-438f-977d-4b26f235ceac](https://www.lucidchart.com/documents/edit/a3cf0c4f-1bc1-438f-977d-4b26f235ceac)
- Workshop Videos: [https://drive.google.com/drive/u/0/folders/0B7z7DpdobBRcY2pnS2FUVTNIVzg](https://drive.google.com/drive/u/0/folders/0B7z7DpdobBRcY2pnS2FUVTNIVzg)

## Start Services

1. clone me
1. init git

		./initGit.sh

1. start Lagoon Services

		docker-compose up -d

1. Follow the Services logs

		docker-compose logs -f

## Start & Test OpenShift

1. start OpenShift

		./startOpenShift.sh

1. test Openshift Node Deployment

		docker-compose exec tests ansible-playbook /ansible/playbooks/node.yaml