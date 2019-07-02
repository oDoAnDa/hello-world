# DevOps: InfraAsCode (IaC) with Ansible

## The Files

![alt text](https://github.com/framgia/infra-standards/blob/master/DevOps/IaC/image-repo/ansible.png)

## Invertory
- Get IP to run Ansible playbook.yml
    - [x] aws-bastion-hosts
    - [x] aws-front-gold-hosts

## Roles
- **Bastion**
    - [x] bastion
    - [x] bastion-to-infra-conf

- **Front-Gold**
    - [x] base
    - [x] ruby
    - [x] nginx
    - [x] puma
    - [ ] project-demo

## Vars
- Get variable for playbook.yml
    - [x] bastion.yml
    - [x] front.yml

## How to Run (Independence)
- **Run on Basion**
    ```
    cd infra-standards/DevOps/IaC/ansible-base/
    ansible-playbook -i ansible-base/inventory/aws-bastion-hosts ansible-base/playbook-bastion.yml
    ```

- **Run on Front**
    ```
    cd infra-standards/DevOps/IaC/ansible-base/
    ansible-playbook -i ansible-base/inventory/aws-front-hosts ansible-base/playbook-front.yml
    ```
