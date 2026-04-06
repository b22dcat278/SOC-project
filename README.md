Security Research Reports

> Tập hợp các báo cáo thực hành về phân tích bảo mật, cấu hình hệ thống phát hiện xâm nhập và phân tích lưu lượng mạng — được thực hiện trong môi trường lab kiểm soát.
Danh sách Báo cáo

1. Phân tích Mã độc TrickBot

TrickBot là một trojan ngân hàng modular nổi tiếng, được sử dụng rộng rãi trong các chiến dịch tấn công APT và ransomware (đặc biệt liên quan đến Ryuk/Conti). Báo cáo này thực hiện phân tích tĩnh và động mẫu mã độc TrickBot trong môi trường sandbox an toàn.

Nội dung chính:
- Tổng quan về TrickBot: lịch sử, mục tiêu, các nhóm đe dọa liên quan
- Phân tích tĩnh (Static Analysis): PE header, strings, import table, entropy
- Phân tích động (Dynamic Analysis): hành vi tiến trình, kết nối mạng, thao tác registry
- Các IOC (Indicators of Compromise) được trích xuất
- Cơ chế persistence

Công cụ sử dụng: PEStudio, Wireshark, Process Monitor, Regshot, VirusTotal

---

2. Cài đặt và Cấu hình Snort IDS

Snort là hệ thống phát hiện/ngăn chặn xâm nhập mã nguồn mở (IDS/IPS) phổ biến nhất hiện nay. Báo cáo này hướng dẫn triển khai Snort từ đầu trên môi trường Linux và xây dựng bộ rule tùy chỉnh để phát hiện các tấn công phổ biến.

Nội dung chính:
- Cài đặt Snort trên Ubuntu 
- Cấu hình file snort.conf: network variables, preprocessors, output plugins
- Triển khai các rule phát hiện
- Kiểm thử rule với traffic
- Phân tích alert log và tích hợp với logging

Công cụ sử dụng: Snort, Ubuntu 22.04, Nmap, Hydra, Kali Linux

---

3. Phân tích Gói tin qua Mạng


Phân tích gói tin là kỹ năng cốt lõi trong điều tra sự cố (Incident Response) và giám sát an ninh mạng. Báo cáo này thực hiện bắt và phân tích lưu lượng mạng thực tế để nhận diện hành vi bất thường và tái dựng hoạt động tấn công.

Nội dung chính:
- Phương pháp luận phân tích gói tin trong SOC
- Bắt lưu lượng với Wireshark và tcpdump
- Phân tích các giao thức: TCP/IP, HTTP, DNS, FTP, ICMP
- Nhận diện dấu hiệu tấn công: SYN flood, ARP spoofing, DNS exfiltration
- Lọc và truy vấn gói tin nâng cao (BPF filters, Wireshark display filters)
- Tái dựng phiên kết nối và trích xuất file từ pcap
- Trường hợp thực tế: phân tích file `.pcap` chứa traffic độc hại

Công cụ sử dụng: Wireshark, tcpdump, tshark, NetworkMiner, Scapy

---

4. Triển khai Splunk để Giám sát và Phát hiện Tấn công

Splunk là nền tảng phân tích log mạnh mẽ, được sử dụng rộng rãi trong SOC để thu thập, tìm kiếm và phát hiện các hành vi bất thường trong hệ thống. Báo cáo này tập trung vào việc triển khai Splunk trong môi trường lab và sử dụng nó để phát hiện các cuộc tấn công mạng thông qua phân tích log.

Nội dung chính:
- Cài đặt Splunk Enterprise trên Linux
- Thu thập log từ nhiều nguồn
- Xây dựng truy vấn SPL (Search Processing Language)
- Phát hiện tấn công Brute-force
- Phát hiện tấn công SQL Injection

Công cụ sử dụng: Splunk Enterprise, Kali Linux, Hydra, sqlmap, Apache, DVWA, Ubuntu Server
