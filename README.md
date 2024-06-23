# A template of ReactTS structure
Template này đã được configure hầu như là đầy đủ các thành phần của một dự án front end cần có. Mình có thể dùng nó để phát triển thêm mà không cần phải cài đặt một số thứ cơ bản nữa.

**Lưu ý**: hiện tại thì template này vẫn đang trong quá trình xây dựng, chưa được ổn định, cho nên cân nhắc trước khi sử dụng.

## Technologies
Template này được xây dựng với các thư viện như là:
- **Tailwindcss** (Styling)
- **React Router Dom** (Routing)
- **Redux/Redux Toolkits** (State Management)
- **Typescript** (Development)
- **Vite** (Development)

## Components
- `apis`: là thành phần mà trong đó mình sẽ dùng để thực hiện các http request.
- `classes` (dự tính bỏ): là thành phần chứa các lớp cơ sở.
- `components`: là thành phần trong đó chứa các UI components dùng để xây dựng trang trong ứng dụng.
- `hooks`: là thành phần chứa các hook can thiệp vào local và global state.
- `layouts` (dự tính bỏ): là thành phần trong đó chứa các UI Component dùng để xây dựng bố cục cho trang hoặc các UI Component nhỏ khác.
- `objects`: là thành phần mà trong đó chứa các đối tượng của ứng dụng như là **user**, là các static class dùng để thao tác.
- `pages`: là thành phần chứa các trang chính trong ứng dụng.
- `routes` (dự tính bỏ): là thành phần chứa các định nghĩa chính cho route.
- `states`: là thành phần trong đó chứa logic để quản lý state trong app, được xây dựng với state manager như `redux`, `react context`, ...
- `themes`: (được config đặc biệt với tailwindcss) là thành phần chứa các chủ đề màu trong ứng dụng.
- `types`: là thành phần chứa các type toàn cục.
- `utils`: là thành phần chứa các helper function.

## Update Plan
Vì template này vẫn chưa hoàn thiện, nên là nó vẫn sẽ có một đợi cập nhật lớn trong năm nay. Cụ thể như là:
- Thêm lớp cơ sở cho apis được xây dựng dựa trên **axios**.
- Chia rõ một UI Component sẽ tách biệt 2 thành phần: xử lý logic bên ngoài và xử lý render bên trong. Cùng với đó là `type` chung cho các component con trong đó.
- Các pages sẽ định nghĩa các route riêng của nó, mang tính nhất quán và rõ ràng hơn.
- Các function helpers nằm trong một static class.
- Thêm các component, logic dùng để kiểm soát lỗi trong ứng dụng.