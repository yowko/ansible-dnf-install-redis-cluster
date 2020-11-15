## 全新安裝

    ```bash
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "purpose=install" main.yml
    ```

## 重新安裝

    > 先 uninstall 並排除安裝基本套件

    ```bash
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "purpose=reinstall" main.yml
    ```

## 更新 config

    ```bash
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini main.yml
    ```

## 升級

    ```
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "purpose=upgrade" main.yml
    ```

## restart service

    ```
    ansible-playbook -i roles/redis-cluster/inventories/dev.ini -e "purpose=restart" main.yml
    ```