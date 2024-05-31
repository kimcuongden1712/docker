?��danh tag latest
danh tag va publish to dockerhub
Work with container
    Create container with name
        docker run -d --name your_container_name your_image_name
    Create container with folder

    Start & stop
    publishing port
    watch logs
    Execute commands in container
    Remove containers
    Using volumes store data container
    Share sourc
        docker run -dp 4202:4200 -v //d/Git/docker/angular-app-docker:/app --name angular3 angular
        docker run -dp 4200:4200 --mount type=bind,source="//d/Git/docker/angular-app-docker",target=/app --name angular angular
Q&A docker
thu tu cau lenh trong docker file ntn la hop ly
khac nhau giua docker run va docker excec
    docker run: lenh nay su dung tao moi 1 container va start container do
    docker exec: lenh nay su dung run command tren 1 container dang chay
--------------
docker compose

PUT và PATCH là hai phương thức HTTP được sử dụng để cập nhật dữ liệu trên máy chủ. Tuy nhiên, chúng có một số khác biệt quan trọng:

PUT được sử dụng để cập nhật toàn bộ tài nguyên. Nếu bạn gửi một yêu cầu PUT tới một tài nguyên cụ thể với một tập hợp dữ liệu, nó sẽ thay thế toàn bộ tài nguyên hiện tại với dữ liệu mới. Điều này có nghĩa là bạn cần cung cấp toàn bộ dữ liệu cho tài nguyên mỗi khi bạn sử dụng PUT.

PATCH được sử dụng để cập nhật một phần của tài nguyên. Nếu bạn gửi một yêu cầu PATCH tới một tài nguyên cụ thể với một tập hợp dữ liệu, nó chỉ cập nhật các phần của tài nguyên đó mà bạn đã chỉ định trong dữ liệu. Điều này có nghĩa là bạn chỉ cần cung cấp dữ liệu cho các phần của tài nguyên mà bạn muốn thay đổi khi sử dụng PATCH.

Ví dụ, giả sử bạn có một tài nguyên người dùng với tên, email và mật khẩu. Nếu bạn muốn thay đổi chỉ email của người dùng, bạn có thể sử dụng PATCH và chỉ cung cấp email mới. Nếu bạn sử dụng PUT, bạn sẽ cần cung cấp tên, email và mật khẩu, ngay cả khi bạn chỉ muốn thay đổi email.