# git

# Cơ bản

### Git la gi? 
- Git là một hệ thống kiểm soát phiên bản phân tán chủ yếu được sử dụng để theo dõi các thay đổi về mã nguồn trong quá trình phát triển phần mềm. Nó cho phép nhiều nhà phát triển cộng tác trong một dự án, theo dõi các sửa đổi được thực hiện đối với cơ sở mã theo thời gian. Được phát triển bởi Linus Torvalds vào năm 2005, Git đã trở thành một trong những hệ thống kiểm soát phiên bản phổ biến nhất nhờ tốc độ, hiệu quả và tính linh hoạt của nó.
  
## Cac thuat ngu trong git
- Repository (Kho chứa): Nơi lưu trữ dự án hoặc mã nguồn
- Commit (Ghi nhận): Hành động lưu trạng thái hiện tại của dự án vào repository.
- Branch (Nhánh): phiên bản riêng của repository, cho phép phát triển độc lập các tính năng không ảnh hưởng đến nhánh chính
- Merge (Hợp nhất): Hành động kết hợp các thay đổi từ một nhánh vào nhánh khác
- Pull request (Yêu cầu kéo): Một yêu cầu để hợp nhất các thay đổi từ một nhánh vào nhánh chính hoặc nhánh khác.
- Push (Đẩy): Hành động gửi các thay đổi từ local repository lên remote repository.
- Pull (Kéo): Hành động cập nhật local repository với các thay đổi mới nhất từ remote repository.
- Clone (Sao chép): Hành động tạo một bản sao của remote repository trên máy cá nhân.
- Fork (Phân nhánh): Hành động tạo ra một bản sao của một repository khác, thường được sử dụng trong các dự án mã nguồn mở.
- Checkout (Chuyển đổi): Hành động chuyển đổi giữa các nhánh hoặc khôi phục trạng thái của các file trong repository.
- Staging (Sân khấu): Vùng chứa các thay đổi đã được chọn để thực hiện commit..
- Conflict (Xung đột): Tình huống khi hai hoặc nhiều thay đổi không thể tự động hợp nhất và cần sự can thiệp thủ công để giải quyết.
- Tag (Nhãn): Một điểm đánh dấu cố định trên lịch sử commit, thường sử dụng để chỉ định các phiên bản phát hành.
- Rebase (Đặt lại cơ sở): Hành động di chuyển tất cả các commit của một nhánh và gắn chúng lên một nhánh khác, sắp xếp lại lịch sử commit.
- Cherry-pick: Hành động chọn lọc và áp dụng một hoặc nhiều commit từ một nhánh sang một nhánh khác.
- Remote (Remote repository): Repository được lưu trữ trên một máy chủ từ xa, thường là nơi mà nhóm làm việc chung lưu trữ mã nguồn
- Submodule (Mô-đun con): Một repository nhỏ được nhúng trong một repository lớn, giúp quản lý mã nguồn từ nhiều nguồn khác nhau.
- Gitignore: Một tệp tin hoặc một bộ quy tắc cho biết những file và thư mục nào không nên được theo dõi bởi Git.

-----------
# Kien truc cua Git

## Working Directory
- Working directory là nơi các file mới được tạo, file cũ bị xóa hoặc nơi thực hiện các thay đổi đối với các file đã có. 
- Sau khi thay đổi được thực hiện, chúng sẽ được thêm vào Staging area. 
  
## Staging Area
- Staging area sẽ chứa một hoặc nhiều file cần được commit. 
- Việc tạo một Commit sẽ khiến Git lấy mã mới từ Staging area và đưa Commit vào Repo chính. 
- Sau đó Commit này sau đó được chuyển đến Commit Area.

## Repository
- Repository, hay Repo, là một kho lưu trữ kỹ thuật số tập trung được các nhà phát triển sử dụng nhằm thực hiện và quản lý các thay đổi đối với mã nguồn của các ứng dụng. 
- Các nhà phát triển phải lưu trữ và chia sẻ những thư mục, tệp văn bản và tài liệu khác trong quá trình phát triển phần mềm.
--------------
# CAC LENH CO BAN CUA GIT

## Git init
- Công dụng: Dùng để khởi tạo 1 git repository cho một dự án mới hoặc đã có sẵn trước đó.
- Cách dùng: Sử dụng  git init trong thư mục gốc của dự án. 

## Git status
- Công dụng: Dùng để kiểm tra trạng thái của file bạn đã thay đổi trong thư mục làm việc của mình. 
- Cách dùng: git status trong thư mục làm việc.

## Git config
- Công dụng: Dùng để đặt user name và email của lập trình viên trong main configuration file. 
- Cách dùng: Dùng để kiểm tra tên và kiểu email trong cấu hình
Kiểm tra tên: git config – global user.name và git config – global user.email
Cài đặt email hoặc tên mới: git config – global user.name = “Hải Nguyễn” và git config – global user.email = “nhulan@gmail.com”

## Git clone
- Công dụng: Dùng git clone để sao chép 1 git repository từ remote source.
- Cách dùng: git clone <:clone git url:>

## Git commit
- Công dụng: Dùng commit giúp Git lưu lại một snapshot bao gồm các sự thay đổi trong thư mục làm việc, các thư mục, tập tin được thay đổi nằm trong Staging Area
- Cách dùng: git commit -m ”Đây là message, bạn dùng để note những thay đổi để sau này dễ dò lại”

## Git add
- Công dụng: Sử dụng git add để đưa tập tinh vào staging area.
- Cách dùng: git add tên_file hoặc muốn thêm tất cả file trong thư mục thì git add all

## Git push/git pull
- Công dụng: Dùng để push hoặc pull các thay đổi đến remote
- Cách dùng: git pull <:remote:> <:branch:> and git push <:remote:> <:branch:>

## Git reset
- Công dụng: Dùng để loại bỏ một tập tin nào đó trong staging area mà không phải bị commit theo. 
- Cách dùng: git reset HEAD tên_file

## Git branch
- Công dụng: Dùng để liệt kê các nhánh trong thư mục
- Cách dùng: git branch hoặc git branch -a

## Git stash
- Công dụng: Dùng để lưu các thay đổi mà lập trình viên chưa muốn commit ngay
- Cách dùng: git stash trong thư mục làm việc.

## Git add
- Công dụng: Dùng để thay đổi stage/index trong thư mục làm việc
- Cách dùng: git add

## Git checkout
- Công dụng: Chuyển sang nhánh khác
- Cách dùng: git checkout <: branch:> hoặc ** _ git checkout -b <: branch:> dùng để tạo và chuyển sang một nhánh mới. 

## Git merge
- Công dụng: Dùng merge hai nhánh lại với nhau
- Cách dùng: Thực hiện chuyển tới branch bạn muốn merge rồi dùng lệnh git merge <:branch_ban_muon_merge:>

## Git remote
- Công dụng: Dùng để check emote/source đa có hoặc thêm remote.
- Cách dùng: git remote để kiểm tra và liệt kê. Và git remote add <: remote_url:> để thêm.



### Xem them thong tin ve git [click here](https://www.w3schools.com/git/)