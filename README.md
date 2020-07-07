# FS_Solution
This's a project trainning FS solution

Solution:
Xác định flex container/item
    - justify-content: 
        space-between; //cách xa đều 1 trái/ 1 phải, space-around: có khoảng cách 2 bên, 
        space-evenly: khoảng cách các item = nhau
    - Flex: 1/ > 1 -> Chiếm hết khoảng không gian theo chiều main axis(ngang)
    -  Flex chia khổi:
        flex 1,2,..: 
    - Flex: mặc định zoom nhỏ thì co width lại
    - flex-wrap: xuống dòng khi co dãn width
      flex-wrap:none/wrap-reverse(đảo ngược khi xuống dòng).
    - căn giữa chiều dọc + ngang-> margin: auto;
    -  align-self: flex-end; reverse trên <-> dưới
    - flex-direction: column/row - reverse: đảo trục
    - Flex: 1 -> Flex-growth/shrink/basis

Oder : Vị trí -> Oder : 1,2, ...

Animation:
    @keyframes name{
    from{
        ....
    }
    to{
        .....
    }
}

    call: animation: name case timeduration;


Fix UI bug:
    1. Navbar font-size
    2. Navbar social-icons
    3. Navbar bell-icons
    4. Notification arrow top offset + z-index + border-radius
    5. Navbar margin beetween avatar + name
    6. User menu separate
    7. Logo link
    8. Search selection offset - top

    9. Header-QR -> z-index
    10. User menu offset-top
    11. Seach history z-index
    12. Cart z-index
    13. Cart product name limit
    14. Category style
    15. product border-radius
https://themify.me/themify-icons


*** Nguyên tắc làm responsive
    .grid {
        .row {
            .column{

            }
            . n -column{

            }
        }

        . n - row{

        }
    }
	
***** Responsive
		- Responsive Web Design (RWD) là xu hướng mới theo đó quy trình thiết kế và phát triển web sẽ đáp ứng mọi thiết bị và môi trường của người dùng theo các tiêu chí kích thước và chiều của màn hình thiết bị
		- Tối ưu trải nghiệm người dùng:
		 + Hiển thị rõ ràng các thành phần
		 + Ẩn/Hiện các thành phần phù hợp theo kích thước màn hình
		 
		- How to:
			using css to hid/show elements
		
		- Tools
			Chrome developerment tools
			Viewport resizer chrome extension
			
		
		** Khái niệm Viewport
			Viewport là khu vực mà người dùng có thể dòm thấy nội dung của trang web. Có thể tạm dịch là KHUNG NHÌN.

		** Media query (@media)
			@media not|only mediatype and (mediafeauture and/or/not mediafeauture{
			
				.....Css code
			}
			
			Keyword: 
				NOT -> Loại trừ
				ONLY -> 
				AND
				OR
			mediatypes: Trường hợp responsive 
				Print -> 
				Screen
				Speech
				ALL
				
			mediafeauture
				MIN-WIDTH: Lớn hơn
				MAX-WIDTH  Lớn hơn
			
			Polyfill: giúp S/dụng được mediaquery
			
		** Khái niệm Breakpoints?
			Breakpoint, là những điểm (chiều rộng màn hình của thiết bị) mà ở đó giao diện được chuyển đổi cho phù hợp với thiết bị hiện tại,
			
			https://responsivedesign.is/develop/browser-feature-support/media-queries-for-common-device-breakpoints/
			
	
			*Moblie: width < 740px *

			*Tablet: width >= 740px and width < 1024 *


			*PC: width >= 1024px *


		** Media queries: Px, rem hay em?
			Sử dụng em


	


		Responsive web design
			grid -> thành phần cha
			row -> dòng
			column -> cột
			getter -> khoảng cách 2 phía của column
			
		layout: 
			PC: 12 col
			Tablet: 8 col
			Mobile: 4 col
	
	***** 	Tạo đối tượng Grid
		Class "grid" giúp chúng ta chứa nội dung chính hoặc các thành phần chính trên layout website.
		Grid được tạo dựng linh động, có thể sử dụng cho trường hợp (full-width) với class "grid" (tượng tự class "container-fluid" trong bootstrap). Và khi muốn sử dụng 1200px Grid system 12 columns các bạn có thể sử dụng 2 class là "grid wide" (tương tự như class "container" trong bootstrap).
		Grid tự động thay đổi chiều rộng trên các thiết bị khác nhau. Để đơn giản hóa việc tạo responsive layout với grid system - ở đây, mình sẽ handle việc tự động thay đổi chiều rộng của "grid" với 3 breakpoints.
	***** 	Tạo đối tượng Row
		Row nghĩa là hàng, được sử dụng để chứa các Columns. Row giúp định hướng các Columns theo chiều ngang. 
		Row sử dụng margin với giá trị âm sang 2 phía trái/phải để "bù trừ" cho khoảng padding trái/phải của Columns (Column padding trái/phải để tạo ra rãnh ngăn - hay còn gọi là gutters).

			
****************************************************************
/* Smartphones (portrait and landscape) ----------- */
@media only screen and (min-device-width : 320px) and (max-device-width : 480px) {
/* Styles */
}

/* Smartphones (landscape) ----------- */
@media only screen and (min-width : 321px) {
/* Styles */
}

/* Smartphones (portrait) ----------- */
@media only screen and (max-width : 320px) {
/* Styles */
}

/* iPads (portrait and landscape) ----------- */
@media only screen and (min-device-width : 768px) and (max-device-width : 1024px) {
/* Styles */
}

/* iPads (landscape) ----------- */
@media only screen and (min-device-width : 768px) and (max-device-width : 1024px) and (orientation : landscape) {
/* Styles */
}

/* iPads (portrait) ----------- */
@media only screen and (min-device-width : 768px) and (max-device-width : 1024px) and (orientation : portrait) {
/* Styles */
}
/**********
iPad 3
**********/
@media only screen and (min-device-width : 768px) and (max-device-width : 1024px) and (orientation : landscape) and (-webkit-min-device-pixel-ratio : 2) {
/* Styles */
}

@media only screen and (min-device-width : 768px) and (max-device-width : 1024px) and (orientation : portrait) and (-webkit-min-device-pixel-ratio : 2) {
/* Styles */
}
/* Desktops and laptops ----------- */
@media only screen  and (min-width : 1224px) {
/* Styles */
}

/* Large screens ----------- */
@media only screen  and (min-width : 1824px) {
/* Styles */
}

/* iPhone 4 ----------- */
@media only screen and (min-device-width : 320px) and (max-device-width : 480px) and (orientation : landscape) and (-webkit-min-device-pixel-ratio : 2) {
/* Styles */
}

@media only screen and (min-device-width : 320px) and (max-device-width : 480px) and (orientation : portrait) and (-webkit-min-device-pixel-ratio : 2) {
/* Styles */
}

/* iPhone 5 ----------- */
@media only screen and (min-device-width: 320px) and (max-device-height: 568px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

@media only screen and (min-device-width: 320px) and (max-device-height: 568px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

/* iPhone 6, 7, 8 ----------- */
@media only screen and (min-device-width: 375px) and (max-device-height: 667px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

@media only screen and (min-device-width: 375px) and (max-device-height: 667px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

/* iPhone 6+, 7+, 8+ ----------- */
@media only screen and (min-device-width: 414px) and (max-device-height: 736px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

@media only screen and (min-device-width: 414px) and (max-device-height: 736px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

/* iPhone X ----------- */
@media only screen and (min-device-width: 375px) and (max-device-height: 812px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

@media only screen and (min-device-width: 375px) and (max-device-height: 812px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

/* iPhone XS Max, XR ----------- */
@media only screen and (min-device-width: 414px) and (max-device-height: 896px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

@media only screen and (min-device-width: 414px) and (max-device-height: 896px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

/* Samsung Galaxy S3 ----------- */
@media only screen and (min-device-width: 320px) and (max-device-height: 640px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

@media only screen and (min-device-width: 320px) and (max-device-height: 640px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 2){
/* Styles */
}

/* Samsung Galaxy S4 ----------- */
@media only screen and (min-device-width: 320px) and (max-device-height: 640px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

@media only screen and (min-device-width: 320px) and (max-device-height: 640px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

/* Samsung Galaxy S5 ----------- */
@media only screen and (min-device-width: 360px) and (max-device-height: 640px) and (orientation : landscape) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

@media only screen and (min-device-width: 360px) and (max-device-height: 640px) and (orientation : portrait) and (-webkit-device-pixel-ratio: 3){
/* Styles */
}

				
		