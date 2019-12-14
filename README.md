# Ruby on Rails on Docker

## 使い方
- 初回起動時  
    ```
    docker-compose up -d && docker-compose run web rake db:create
    ```

- ２回目以降動時  
    ```
    docker-compose up -d
    ```

- ソースを変更したとき  
    ```
    # 細かいところは好み
    docker-compose down --rmi all && docker-compose up -build
    ```

- 止めるとき 
    ```
    docker-compose down -v
    ```

    - イメージごと消したいとき  
        ```
        docker-compose down --rmi all
        ```

