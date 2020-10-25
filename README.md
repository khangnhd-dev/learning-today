# 25/10/2020
## Clean Code
https://github.com/nguyentranchung/clean-code-php#tr%C3%A1nh-%C4%91i%E1%BB%81u-ki%E1%BB%87n-ph%E1%BB%A7-%C4%91%E1%BB%8Bnh
- Tránh dùng điều kiện
- Tránh kiểm tra kiểu dữ liệu (phần 1) dùng interface
`

    
    <?php 
    
      interface Traveler{
          public function go();
      }
    
      class Bicycle implements Traveler{
        public function go(){
          echo "go Bicycle";
        }
      }
    
      class Car implements Traveler{
        public function go(){
          echo "go by cars";
        }
      }
    
      function travelToTexas(Traveler $traveler){
          $traveler->go();
      }
    
      travelToTexas(new Bicycle());
      travelToTexas(new Car());`
      
- Tránh kiểm tra kiểu dữ liệu (phần 2)
- Xóa dead code
