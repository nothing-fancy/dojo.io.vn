---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: "Sản phẩm"
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image:  /assets/img/splash/splash.jpg
  actions:
    - label: "Khoá học"
      url: "/courses"
    - label: "Hệ thống thực hành"
      url: "#"
    - label: "Đọc sách trên mây"
      url: "#"

  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
excerpt: "Nắm bắt các công nghệ mới với **DojoIO**.<br> Ở đây có các khóa học chất lượng, hệ thống thực hành, và tài nguyên học tập."
intro:
  - title: Dự án của tôi
feature_row_dtcn:
  - image_path: /assets/img/splash/dtcn.png
    alt: "Giảng dạy trực tuyến cho người mới làm quen với Điện toán đám mây AWS"
    title: "Làm chủ nền tảng Amazon Web Services với chứng chỉ AWS Solution Architect Associate"
    excerpt: >-
      Khoá học này phù hợp cho những người mới bắt đầu với Điện toán đám mây và mong muốn hiểu rõ về Amazon Web Services (AWS), một trong những nền tảng điện toán đám mây hàng đầu trên thế giới. Với sự phổ biến của AWS trong ngành công nghiệp hiện nay, việc hiểu biết và làm chủ các dịch vụ của nó là một lợi thế lớn cho bất kỳ ai muốn theo đuổi sự nghiệp trong lĩnh vực công nghệ thông tin.
    url: "#test-link"
    btn_label: "Xem thông tin chi tiết"
    btn_class: "btn--primary"
feature_row_dtdn:
  - image_path: /assets/img/splash/dtdn.png
    alt: "Giảng dạy cho PTTC1, Học viện Công nghệ Bưu Chính Viễn Thông"
    title: "Đào tạo nhân lực có kỹ năng sử dụng điện toán đám mây AWS cho doanh nghiệp"
    excerpt: >-
      Khoá học này là một chương trình huấn luyện đặc biệt được thiết kế để cung cấp kỹ năng sử dụng điện toán đám mây AWS cho nhân lực trong các doanh nghiệp. Với sự gia tăng không ngừng của công nghệ điện toán đám mây và vai trò quan trọng của AWS trong việc cung cấp dịch vụ đám mây hàng đầu, việc có nhân viên được đào tạo vững vàng về AWS trở nên cực kỳ quan trọng để tối ưu hóa hiệu suất và cạnh tranh của doanh nghiệp.
feature_row_dtcm:
  - image_path: /assets/img/splash/dtcm.png
    alt: "Đào tạo chuyên môn cho kỹ sư Full-stack"
    title: "Đào tạo kỹ sư Full-stack"
    excerpt: >-
      Khoá học là một chương trình huấn luyện toàn diện nhằm phát triển năng lực chuyên môn và kỹ năng thực hành cho các nhà phát triển web. Với sự phát triển không ngừng của công nghệ Web hiện nay, kỹ sư Full-stack trở thành một yếu tố then chốt trong việc xây dựng các ứng dụng web đa dạng và hiệu quả.

---
{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row_dtcn"  type="right" %}
{% include feature_row id="feature_row_dtdn"  type="left" %}
{% include feature_row id="feature_row_dtcm"  type="right" %}
