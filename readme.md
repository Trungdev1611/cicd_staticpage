Với static page ta không cần build và cài đặt npm

các bước
B1. Tạo static page html, css, có thể sử dụng github page để deploy,
   Ta thấy khi ta update code mới, trang web đã deploy không tự động cập nhật code mới 

=>> thêm cicd để tự động cập nhật code mới khi push

B2. thêm thư mục .github/workflows và tạo file deploy.yaml
B3. push code lên, lúc này vì có file deploy.yaml rồi nên github action tự động phát hiện và làm theo các chỉ dẫn trong file

docker file thì viết để tạo ra image để đưa lên các nền tảng, trong khi yaml  trong workflow thì tạo ra để deploy tự động với github action