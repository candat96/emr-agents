# Danh sach tinh nang EMR chuan quoc te

> **Tong cong: ~400 features** | **16 modules** | **Tieu chuan: HL7 FHIR R4, ICD-10, LOINC, SNOMED CT**

---

## Tong quan modules

| # | Module | So luong | Mo ta |
|---|--------|----------|-------|
| 1 | [Quan ly benh nhan](#1-quan-ly-benh-nhan) | 30 | Ho so, bao hiem, tien su, di ung |
| 2 | [Lich hen & Xep lich](#2-lich-hen--xep-lich) | 30 | Dat lich, hang doi, nhac hen, lich bac si |
| 3 | [Benh an dien tu (EMR)](#3-benh-an-dien-tu-emr) | 60 | SOAP note, chan doan, dieu tri, chuyen khoa |
| 4 | [Don thuoc & Duoc](#4-don-thuoc--duoc) | 40 | Ke don, tuong tac thuoc, ton kho duoc |
| 5 | [Xet nghiem](#5-xet-nghiem) | 30 | Chi dinh, mau benh pham, ket qua, LIS |
| 6 | [Chan doan hinh anh](#6-chan-doan-hinh-anh) | 20 | DICOM, PACS, doc ket qua, luu tru |
| 7 | [Thanh toan & Hoa don](#7-thanh-toan--hoa-don) | 25 | Vien phi, bao hiem, hoan tra, bao cao |
| 8 | [Ton kho](#8-ton-kho) | 20 | Thuoc, vat tu, nhap xuat, han dung |
| 9 | [Bao cao & Phan tich](#9-bao-cao--phan-tich) | 20 | Dashboard, KPI, du bao, BI |
| 10 | [Quan tri he thong](#10-quan-tri-he-thong) | 15 | User, role, cau hinh, audit log |
| 11 | [Telemedicine](#11-telemedicine) | 20 | Video call, tu van tu xa, IoT |
| 12 | [Cong benh nhan & Mobile](#12-cong-benh-nhan--mobile) | 25 | Portal, app, dat lich, xem ket qua |
| 13 | [Tich hop & Lien thong](#13-tich-hop--lien-thong) | 25 | HL7, FHIR, BHXH, SSO, webhook |
| 14 | [Dieu duong & Quan ly buong](#14-dieu-duong--quan-ly-buong) | 25 | Giuong benh, MAR, ban giao ca |
| 15 | [Phong mo & Phau thuat](#15-phong-mo--phau-thuat) | 20 | Lich mo, WHO checklist, gay me, hoi suc |
| 16 | [Tuan thu & Bao mat](#16-tuan-thu--bao-mat) | 20 | RBAC, MFA, ma hoa, DPIA |

---

## 1. Quan ly benh nhan

> **30 features** — Quan ly toan bo thong tin hanh chinh, bao hiem, tien su benh nhan

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Tao ho so benh nhan | Dang ky benh nhan moi voi day du thong tin nhan khau |
| 2 | Cap nhat ho so benh nhan | Chinh sua thong tin hanh chinh, lien he |
| 3 | Tim kiem benh nhan | Tim theo ten, ma benh nhan, CCCD, SDT |
| 4 | Gop ho so trung | Phat hien va merge ho so benh nhan bi trung lap |
| 5 | Quan ly nhan khau hoc | Quan ly thong tin dan toc, nghe nghiep, dia chi |
| 6 | Quan ly thong tin bao hiem | BHYT, bao hiem tu nhan, han the |
| 7 | Quan ly lien he khan cap | Thong tin nguoi than, nguoi lien he khan cap |
| 8 | Quan ly tien su benh | Tien su benh ly ca nhan |
| 9 | Quan ly tien su gia dinh | Tien su benh ly gia dinh (di truyen) |
| 10 | Quan ly di ung | Danh sach di ung thuoc, thuc pham, hoa chat |
| 11 | Quan ly thuoc dang dung | Danh sach thuoc benh nhan dang su dung |
| 12 | Anh benh nhan | Chup va luu anh chan dung benh nhan |
| 13 | Upload tai lieu | Tai len giay to, ket qua xet nghiem cu |
| 14 | Phieu dong y dieu tri | Quan ly consent form theo quy dinh |
| 15 | Dong y quyen rieng tu | Consent ve bao mat thong tin ca nhan |
| 16 | Gan nhan benh nhan | Tag phan loai: VIP, uu tien, canh bao |
| 17 | Ghi chu benh nhan | Note noi bo cua nhan vien y te |
| 18 | Timeline benh nhan | Dong thoi gian lich su kham chua benh |
| 19 | Nguon gioi thieu | Theo doi nguon gioi thieu benh nhan den |
| 20 | Phan nhom benh nhan | Phan nhom theo benh ly, do tuoi, khu vuc |
| 21 | Danh sach chan | Chan benh nhan vi pham noi quy |
| 22 | Quan he benh nhan | Lien ket gia dinh (vo/chong, con, bo me) |
| 23 | Truy cap Patient Portal | Cap quyen dang nhap cong benh nhan |
| 24 | Ma QR benh nhan | Tao QR code dinh danh nhanh |
| 25 | Ma dinh danh duy nhat | Ma benh nhan duy nhat toan he thong |
| 26 | Kiem tra quyen loi BHYT | Tra cuu truc tuyen tinh trang the BHYT |
| 27 | Phat hien ho so trung | Tu dong canh bao ho so co nghi ngo trung |
| 28 | Phan tich nhan khau hoc | Thong ke do tuoi, gioi tinh, khu vuc |
| 29 | Tuy chon lien lac | Email, SMS, Zalo — kenh lien lac uu tien |
| 30 | Quan ly trang thai | Dang dieu tri, xuat vien, chuyen vien, tu vong |

---

## 2. Lich hen & Xep lich

> **30 features** — Quan ly lich kham, hang doi, nhac hen tu dong

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Quan ly lich bac si | Cai dat gio lam viec, nghi phep tung bac si |
| 2 | Quan ly lich phong kham | Lich hoat dong phong kham theo ngay/tuan |
| 3 | Dat lich hen | Dat lich kham cho benh nhan |
| 4 | Huy lich hen | Huy bo lich hen da dat |
| 5 | Doi lich hen | Chuyen doi ngay/gio hen kham |
| 6 | Nhac hen qua SMS | Gui SMS nhac lich hen tu dong |
| 7 | Nhac hen qua email | Gui email nhac lich hen tu dong |
| 8 | Danh sach cho | Quan ly benh nhan cho khi het slot |
| 9 | Dat lich online | Benh nhan tu dat lich qua website/app |
| 10 | Quan ly hang doi | So thu tu, man hinh goi so |
| 11 | Tinh trang bac si | Hien thi bac si dang ranh/ban/nghi |
| 12 | Xep lich da co so | Dat lich tai nhieu co so phong kham |
| 13 | Lich hen dinh ky | Hen tai kham dinh ky tu dong |
| 14 | Xac nhan lich hen | Benh nhan xac nhan qua SMS/app |
| 15 | Check-in benh nhan | Dang ky co mat tai quay le tan |
| 16 | Check-out benh nhan | Ket thuc luot kham, chuyen thanh toan |
| 17 | Phan tich lich hen | Thong ke ty le huy, no-show, tai kham |
| 18 | Lich hen dang calendar | Hien thi lich hen theo ngay/tuan/thang |
| 19 | Quan ly slot | Cai dat so luong slot moi khung gio |
| 20 | Phat hien xung dot | Canh bao trung lich bac si/phong |
| 21 | Ghi chu lich hen | Note yeu cau dac biet cua benh nhan |
| 22 | Phan loai lich hen | Kham moi, tai kham, cap cuu, tu van |
| 23 | Thoi luong kham | Cai dat thoi gian kham tung loai |
| 24 | Theo doi no-show | Ghi nhan benh nhan vang mat khong bao |
| 25 | Hen kham tu xa | Dat lich kham telemedicine |
| 26 | Dat nhieu bac si | Hen kham voi nhieu bac si trong 1 luot |
| 27 | Dashboard lich hen | Tong quan lich hen trong ngay |
| 28 | Theo doi trang thai | Cho kham, dang kham, da kham, huy |
| 29 | Quan ly cong suat | Gioi han so benh nhan toi da/ngay |
| 30 | Bao cao lich hen | Bao cao chi tiet theo bac si, phong kham |

---

## 3. Benh an dien tu (EMR)

> **60 features** — Module lon nhat — ghi nhan, chan doan, dieu tri, theo doi lam sang

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Tao luot kham | Khoi tao encounter moi cho benh nhan |
| 2 | SOAP Note | Ghi nhan theo chuan Subjective-Objective-Assessment-Plan |
| 3 | Template lam sang | Mau benh an theo chuyen khoa |
| 4 | Danh sach van de | Problem list theo doi cac van de suc khoe |
| 5 | Nhap chan doan | Ghi chan doan chinh, phu |
| 6 | Ma hoa ICD | Gan ma ICD-10 cho chan doan |
| 7 | Soan thao ghi chu | Editor ghi chu lam sang (rich text) |
| 8 | Nhap sinh hieu | Nhiet do, huyet ap, mach, SpO2, can nang |
| 9 | Kham the luc | Ghi nhan kham toan than, co quan |
| 10 | Hoi benh he thong | Review of Systems theo co quan |
| 11 | Canh bao lam sang | Alert di ung, tuong tac thuoc, ket qua bat thuong |
| 12 | Kiem tra di ung | Tu dong kiem tra di ung khi ke don |
| 13 | Kiem tra tuong tac thuoc | Canh bao tuong tac thuoc-thuoc |
| 14 | Ho tro phac do | Goi y phac do dieu tri theo chan doan |
| 15 | Ke hoach dieu tri | Lap ke hoach dieu tri tong the |
| 16 | Ke hoach tai kham | Hen lich tai kham, theo doi |
| 17 | Huong dan benh nhan | In/gui huong dan cham soc tai nha |
| 18 | Giay ra vien | Tao tom tat ra vien |
| 19 | Giay chuyen vien | Tao giay gioi thieu chuyen tuyen |
| 20 | Dinh kem lam sang | Dinh kem file, hinh anh vao benh an |
| 21 | Chup anh lam sang | Chup va luu anh ton thuong, thuong tich |
| 22 | Ho so y te co cau truc | Du lieu co cau truc theo chuan FHIR |
| 23 | Giong noi thanh van ban | Nhan dang giong noi de ghi benh an |
| 24 | Tom tat luot kham | Tu dong tao tom tat encounter |
| 25 | Timeline lam sang | Dong thoi gian toan bo lich su dieu tri |
| 26 | Xem lai tien su | Review toan bo tien su benh ly |
| 27 | Doi chieu thuoc | So sanh thuoc truoc/sau nhap vien |
| 28 | Ho tro quyet dinh lam sang | CDS — goi y dua tren evidence-based |
| 29 | Nhat ky kiem soat | Audit trail moi thao tac tren benh an |
| 30 | Lien trinh cham soc | Care pathway theo benh ly |
| 31 | Phan loai cap cuu | Triage assessment tai phong cap cuu |
| 32 | Danh gia dieu duong | Phieu danh gia dieu duong |
| 33 | Danh gia bac si | Phieu danh gia cua bac si dieu tri |
| 34 | Ghi nhan thu thuat | Tai lieu hoa thu thuat, tieu phau |
| 35 | Mau tai lieu lam sang | Template giay to lam sang |
| 36 | Smart Forms | Bieu mau thong minh tu dong dien |
| 37 | Smart Macros | Phim tat nhap nhanh cum tu thuong dung |
| 38 | Goi y ma benh | Tu dong goi y ICD-10 tu mo ta |
| 39 | So dang ky benh | Registry theo doi benh truyen nhiem, man tinh |
| 40 | Cong tac nhom dieu tri | Phoi hop lien chuyen khoa |
| 41 | Ky so tai lieu y te | Chu ky dien tu tren benh an |
| 42 | Quan ly phien ban benh an | Version control du lieu lam sang |
| 43 | Theo doi benh man tinh | Quan ly dai han: dai thao duong, tang HA |
| 44 | Lich su tiem chung | Ghi nhan vaccine da tiem |
| 45 | Theo doi thai ky | San khoa — theo doi thai ky |
| 46 | Bieu do tang truong nhi | Growth chart cho tre em |
| 47 | Ho so ung buou | Benh an chuyen khoa ung thu |
| 48 | So do rang | Dental chart cho rang ham mat |
| 49 | Hinh anh da lieu | Chup va so sanh ton thuong da |
| 50 | Template chuyen khoa | Mau benh an rieng theo tung chuyen khoa |
| 51 | Cham diem nguy co | Scoring: NEWS, APACHE, qSOFA... |
| 52 | Gan nhan luot kham | Tag encounter: cap cuu, VIP, nghien cuu |
| 53 | Tu dong hoa quy trinh | Workflow automation lam sang |
| 54 | Quan ly ca benh | Case management phuc tap |
| 55 | Ghi chu lien chuyen khoa | Note da chuyen khoa trong 1 benh an |
| 56 | KPI lam sang | Theo doi chi so chat luong lam sang |
| 57 | Theo doi tien trinh | Bieu do tien trinh dieu tri benh nhan |
| 58 | Xuat tom tat lam sang | Export benh an ra PDF/FHIR |
| 59 | Theo doi chuyen vien | Trang thai giay chuyen tuyen |
| 60 | Quan ly dot dieu tri | Care episode tu nhap vien den ra vien |

---

## 4. Don thuoc & Duoc

> **40 features** — Ke don dien tu, kiem soat tuong tac, quan ly duoc

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Ke don dien tu | Tao don thuoc dien tu (ePrescription) |
| 2 | Danh muc thuoc | Catalog thuoc theo ten goc, ten thuong mai |
| 3 | Tinh lieu dung | Tu dong tinh lieu theo can nang, tuoi |
| 4 | Kiem tra tuong tac thuoc | Canh bao tuong tac thuoc-thuoc |
| 5 | Kiem tra di ung thuoc | Canh bao di ung khi ke don |
| 6 | Mau don thuoc | Template don thuoc theo chan doan |
| 7 | Ke don tiep | Refill don thuoc cu |
| 8 | Huy don thuoc | Huy bo don thuoc da ke |
| 9 | Duyet don thuoc | Phe duyet don boi duoc si |
| 10 | Lich su dung thuoc | Toan bo lich su thuoc da dung |
| 11 | Theo doi tuan thu thuoc | Do luong benh nhan uong thuoc dung lich |
| 12 | Xu ly don tai nha thuoc | Quy trinh nhan don, cap phat |
| 13 | Tich hop ton kho thuoc | Kiem tra ton truoc khi ke |
| 14 | Quet barcode thuoc | Xac nhan thuoc bang ma vach |
| 15 | Cap phat thuoc | Ghi nhan phat thuoc cho benh nhan |
| 16 | Thay the thuoc | Doi thuoc tuong duong khi het hang |
| 17 | Canh bao thuoc | Alert qua lieu, chong chi dinh |
| 18 | Phac do dung thuoc | Tich hop guideline dung thuoc quoc te |
| 19 | Quan ly thuoc kiem soat | Thuoc gay nghien, huong than dac biet |
| 20 | In don thuoc | In don thuoc theo mau quy dinh |
| 21 | Chu ky so don thuoc | Ky dien tu xac nhan don thuoc |
| 22 | Doi chieu thuoc | Medication reconciliation nhap/xuat vien |
| 23 | Ghi nhan tu van thuoc | Noi dung tu van cho benh nhan |
| 24 | Phan tich don thuoc | Thong ke xu huong ke don |
| 25 | Danh muc thuoc BV | Formulary thuoc duoc phep su dung |
| 26 | Xac nhan thuoc BHYT | Kiem tra thuoc thuoc danh muc BHYT |
| 27 | Nhac uong thuoc | Push notification nhac gio uong |
| 28 | Kiem tra han dung | Canh bao thuoc gan/het han |
| 29 | Theo doi lo thuoc | Truy xuat nguon goc theo batch |
| 30 | Canh bao ton kho duoc | Alert khi thuoc sap het |
| 31 | Tra thuoc | Quy trinh benh nhan tra thuoc |
| 32 | Xu ly thuoc huy | Quan ly thuoc huy, het han |
| 33 | KPI nha thuoc | Hieu suat hoat dong nha thuoc |
| 34 | Kiem soat doi chieu thuoc | Audit quy trinh medication reconciliation |
| 35 | Bao cao duoc | Bao cao su dung thuoc dinh ky |
| 36 | Dashboard tuong tac thuoc | Tong quan canh bao tuong tac |
| 37 | Quan ly khang sinh | Antibiotic stewardship tracking |
| 38 | Phan tich chi phi thuoc | So sanh chi phi thuoc theo chan doan |
| 39 | Giao duc benh nhan ve thuoc | Tai lieu huong dan su dung thuoc |
| 40 | Lich su chi dinh thuoc | Toan bo order thuoc da ke |

---

## 5. Xet nghiem

> **30 features** — Chi dinh, thu mau, ket qua, tich hop LIS

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Tao chi dinh xet nghiem | Bac si chi dinh xet nghiem |
| 2 | Danh muc xet nghiem | Catalog xet nghiem co san |
| 3 | Theo doi mau benh pham | Tracking specimen tu thu den ket qua |
| 4 | Dan barcode mau | In ma vach cho ong mau |
| 5 | Thu mau benh pham | Ghi nhan quy trinh lay mau |
| 6 | Quan ly quy trinh lab | Workflow toan bo quy trinh xet nghiem |
| 7 | Nhap ket qua | Ky thuat vien nhap ket qua |
| 8 | Xac nhan ket qua | Validation ket qua boi ky thuat vien cap cao |
| 9 | Duyet ket qua | Bac si lab phe duyet tra ket qua |
| 10 | Canh bao ket qua bat thuong | Alert khi chi so ngoai khoang tham chieu |
| 11 | Dinh kem ket qua | Gan file PDF, hinh anh vao ket qua |
| 12 | Tich hop thiet bi | Ket noi truc tiep may xet nghiem |
| 13 | Tich hop LIS | Lien thong voi he thong Lab Information System |
| 14 | Quan ly khoang tham chieu | Cai dat reference range theo tuoi, gioi |
| 15 | Bieu do xu huong | Trend chart theo doi chi so theo thoi gian |
| 16 | Canh bao gia tri nguy hiem | Critical value alert bao bac si ngay |
| 17 | Theo doi thoi gian xu ly | TAT — turnaround time moi xet nghiem |
| 18 | Uu tien xet nghiem | Cap do uu tien: thuong, khan, cap cuu |
| 19 | Xu ly theo lo | Chay xet nghiem theo batch |
| 20 | Theo doi trang thai chi dinh | Trang thai: da chi dinh, dang xu ly, co ket qua |
| 21 | Tich hop thanh toan lab | Lien ket chi phi xet nghiem voi vien phi |
| 22 | Chia se ket qua | Gui ket qua cho bac si dieu tri/benh nhan |
| 23 | Tao bao cao xet nghiem | In phieu ket qua xet nghiem |
| 24 | Kiem soat chat luong | QC noi kiem, ngoai kiem |
| 25 | Nhat ky kiem soat lab | Audit trail thao tac trong lab |
| 26 | Xuat ket qua | Export ket qua ra PDF, CSV |
| 27 | Dashboard phan tich lab | Thong ke hoat dong lab |
| 28 | Bao cao nang suat | Hieu suat ky thuat vien, may moc |
| 29 | Huy chi dinh | Huy bo chi dinh xet nghiem |
| 30 | Sua chi dinh | Chinh sua chi dinh da tao |

---

## 6. Chan doan hinh anh

> **20 features** — DICOM, PACS, doc ket qua, luu tru hinh anh y te

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Chi dinh CDHA | Bac si chi dinh chup X-quang, CT, MRI... |
| 2 | Quan ly modality | Cai dat may chup: X-ray, CT, MRI, US |
| 3 | Quy trinh X-quang | Workflow tu chi dinh den tra ket qua |
| 4 | Bao cao X-quang | Bac si CDHA doc va tra ket qua |
| 5 | Trinh xem hinh anh | Viewer xem anh DICOM tren web |
| 6 | Tich hop DICOM | Nhan anh tu may chup qua giao thuc DICOM |
| 7 | Tich hop PACS | Ket noi he thong luu tru hinh anh |
| 8 | Ghi chu tren hinh anh | Annotation: do, danh dau, ghi chu |
| 9 | So sanh hinh anh | So sanh anh truoc/sau dieu tri |
| 10 | Dinh kem hinh anh | Gan anh vao benh an |
| 11 | Duyet bao cao CDHA | Phe duyet ket qua CDHA |
| 12 | Canh bao nguy hien | Alert ket qua bat thuong nguy hiem |
| 13 | Trang thai chi dinh | Theo doi: da chi dinh, da chup, co ket qua |
| 14 | Thanh toan CDHA | Lien ket chi phi CDHA voi vien phi |
| 15 | Phan tich CDHA | Thong ke so luong, loai chup |
| 16 | Luu tru hinh anh | Archive anh dai han |
| 17 | Chia se hinh anh | Gui anh cho bac si khac/benh nhan |
| 18 | Kiem soat chat luong | QC hinh anh va bao cao |
| 19 | Nhat ky kiem soat | Audit log thao tac CDHA |
| 20 | Xuat ket qua | Export bao cao ra PDF |

---

## 7. Thanh toan & Hoa don

> **25 features** — Quan ly vien phi, bao hiem, hoan tra, bao cao tai chinh

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Danh muc dich vu | Catalog dich vu kham, thu thuat, xet nghiem |
| 2 | Quan ly bang gia | Cai dat gia theo doi tuong, loai dich vu |
| 3 | Tao phieu thu | Lap phieu thu vien phi |
| 4 | Dieu chinh vien phi | Sua lai chi phi khi co sai sot |
| 5 | Giam gia/mien giam | Ap dung giam gia, mien phi theo chinh sach |
| 6 | Xuat hoa don | Tao hoa don dien tu/giay |
| 7 | Ghi nhan thanh toan | Thu tien mat, chuyen khoan, the |
| 8 | Phuong thuc thanh toan | Tien mat, the, QR Pay, vi dien tu |
| 9 | Thanh toan bao hiem | Xu ly phan BHYT chi tra |
| 10 | Tinh dong chi tra | Tu dong tinh phan benh nhan dong |
| 11 | Tao ho so bao hiem | Tao claim gui co quan bao hiem |
| 12 | Theo doi claim | Trang thai claim: gui, duyet, tu choi |
| 13 | Hoan tra | Hoan tien khi huy dich vu |
| 14 | Huy phieu thu | Huy bo phieu thu sai |
| 15 | Dashboard doanh thu | Tong quan doanh thu theo ngay/thang |
| 16 | Kiem toan vien phi | Audit phieu thu, hoa don |
| 17 | Bao cao doanh thu ngay | Ket ca, doi soat cuoi ngay |
| 18 | Doanh thu theo khoa | Phan tich doanh thu tung khoa/phong |
| 19 | Chia se doanh thu bac si | Tinh hoa hong, thu nhap bac si |
| 20 | Phan tich tai chinh | Thong ke xu huong doanh thu |
| 21 | Tinh thue | Thue GTGT, thue thu nhap |
| 22 | Xuat du lieu | Export bao cao ra Excel, PDF |
| 23 | Bao cao tai chinh | Bao cao tai chinh tong hop |
| 24 | Tich hop cong thanh toan | Ket noi VNPay, Momo, ngan hang |
| 25 | Doi soat | Reconciliation so sach hang ngay |

---

## 8. Ton kho

> **20 features** — Quan ly thuoc, vat tu, nhap xuat, han dung

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Ton kho thuoc | Quan ly so luong thuoc hien co |
| 2 | Ton kho vat tu y te | Quan ly vat tu tieu hao, thiet bi |
| 3 | Quan ly kho | Cai dat nhieu kho: kho chinh, kho le, kho khoa |
| 4 | Nhap xuat kho | Ghi nhan phieu nhap, phieu xuat |
| 5 | Theo doi lo | Quan ly batch/lot number |
| 6 | Theo doi han dung | Canh bao thuoc/vat tu gan het han |
| 7 | Canh bao ton kho | Alert khi duoi muc ton toi thieu |
| 8 | Chuyen kho | Dieu chuyen giua cac kho |
| 9 | Dieu chinh ton kho | Xu ly chenh lech kiem ke |
| 10 | Dat hang | Tao don dat hang nha cung cap |
| 11 | Quan ly nha cung cap | Danh sach NCC, hop dong, gia |
| 12 | Dinh gia ton kho | Tinh gia tri ton kho (FIFO, binh quan) |
| 13 | Bao cao ton kho | Bao cao nhap xuat ton |
| 14 | Barcode ton kho | Ma vach cho thuoc, vat tu |
| 15 | Kiem ke | Kiem ke dinh ky, dot xuat |
| 16 | Phan tich ton kho | Thong ke tieu thu, ton dong |
| 17 | Tich hop nha thuoc | Dong bo ton kho voi nha thuoc |
| 18 | Goi y dat hang | Tu dong de xuat dat hang khi ton thap |
| 19 | Bao cao su dung | Thong ke luong tieu thu theo thoi gian |
| 20 | Dashboard ton kho | Tong quan ton kho realtime |

---

## 9. Bao cao & Phan tich

> **20 features** — Dashboard, KPI, du bao, ket noi BI

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Dashboard van hanh | Tong quan hoat dong benh vien theo ngay |
| 2 | KPI lam sang | Chi so chat luong kham chua benh |
| 3 | KPI tai chinh | Chi so doanh thu, cong no, loi nhuan |
| 4 | Phan tich benh nhan | Thong ke benh nhan theo nhom |
| 5 | Hieu suat bac si | So luot kham, doanh thu, danh gia |
| 6 | Thong ke benh tat | Phan bo benh theo ICD-10 |
| 7 | Phan tich don thuoc | Xu huong ke don, chi phi thuoc |
| 8 | Phan tich lich hen | Ty le dat lich, huy, no-show |
| 9 | Phan tich doanh thu | Xu huong doanh thu theo thoi gian |
| 10 | Phan tich ton kho | Tieu thu, ton dong, qua han |
| 11 | Phan tich xet nghiem | Thong ke loai XN, ty le bat thuong |
| 12 | Phan tich CDHA | Thong ke loai chup, thoi gian doc |
| 13 | Phan tich cohort | So sanh nhom benh nhan |
| 14 | Phan tich luu giu BN | Ty le benh nhan quay lai |
| 15 | Phan tich hai long | Khao sat muc do hai long |
| 16 | Phan tich du bao | Predictive: du bao luot kham, doanh thu |
| 17 | Tich hop BI | Ket noi Power BI, Metabase, Superset |
| 18 | Xuat du lieu | Export CSV, Excel, PDF |
| 19 | Tao bao cao tuy chinh | Drag & drop report builder |
| 20 | Gui bao cao tu dong | Gui bao cao dinh ky qua email |

---

## 10. Quan tri he thong

> **15 features** — Quan ly nguoi dung, phan quyen, cau hinh

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Quan ly nguoi dung | Tao, sua, khoa tai khoan nhan vien |
| 2 | Quan ly vai tro | Dinh nghia role: bac si, dieu duong, admin... |
| 3 | Quan ly quyen | Phan quyen chi tiet theo chuc nang |
| 4 | Nhat ky he thong | Audit log moi thao tac |
| 5 | Quan ly to chuc | Cau hinh benh vien, phong kham |
| 6 | Quan ly phong kham | Thong tin co so, dia chi, lien he |
| 7 | Quan ly khoa phong | Cau truc khoa, phong, don vi |
| 8 | Quan ly cau hinh | Tham so he thong, tuy chon |
| 9 | Quan ly mau bieu | Template don thuoc, giay to, bao cao |
| 10 | Quan ly danh muc goc | Master data: ICD, thuoc, dich vu |
| 11 | Cau hinh thong bao | Cai dat kenh va noi dung thong bao |
| 12 | Cau hinh tich hop | Quan ly ket noi API ben ngoai |
| 13 | Sao luu du lieu | Backup dinh ky, phuc hoi |
| 14 | Giam sat he thong | Health check, uptime, performance |
| 15 | Quan ly license | Ban quyen, han su dung, module |

---

## 11. Telemedicine

> **20 features** — Kham tu xa, video call, theo doi IoT

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Tu van video | Kham benh qua video call |
| 2 | Tu van audio | Kham benh qua dien thoai/audio |
| 3 | Dat lich telemedicine | Xep lich kham tu xa |
| 4 | Phong cho tu xa | Waiting room ao truoc khi vao phong kham |
| 5 | Chia se man hinh | Bac si chia se hinh anh, ket qua cho BN |
| 6 | Dong y kham tu xa | Consent form kham telemedicine |
| 7 | Ke don tu xa | Ke don dien tu sau kham online |
| 8 | Theo doi sinh hieu tu xa | Nhan du lieu tu thiet bi tai nha |
| 9 | Tich hop thiet bi deo | Ket noi smartwatch, may do huyet ap |
| 10 | Ghi hinh buoi kham | Luu lai video buoi tu van |
| 11 | Ghi chu telemedicine | Note bac si trong buoi kham tu xa |
| 12 | Tai kham tu xa | Hen lich tai kham telemedicine |
| 13 | Thanh toan telemedicine | Thu phi kham tu xa |
| 14 | Phan tich telemedicine | Thong ke luot kham online |
| 15 | Hoi chan nhieu bac si | Hoi chan tu xa nhieu chuyen gia |
| 16 | Hang doi telemedicine | Quan ly thu tu benh nhan cho |
| 17 | Thong bao telemedicine | Push thong bao den gio kham |
| 18 | Check-in telemedicine | Benh nhan bao co mat online |
| 19 | Kiem tra ky thuat | Test camera, mic truoc khi kham |
| 20 | Khao sat hai long | Danh gia chat luong sau kham tu xa |

---

## 12. Cong benh nhan & Mobile

> **25 features** — Patient portal, ung dung di dong cho benh nhan

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Dang nhap/dang ky | Benh nhan tao tai khoan va dang nhap |
| 2 | Xem ho so suc khoe | Benh nhan xem benh an cua minh |
| 3 | Xem ket qua xet nghiem | Tra cuu ket qua lab online |
| 4 | Xem ket qua CDHA | Xem anh chup va ket qua CDHA |
| 5 | Dat lich hen online | Tu dat lich kham qua app |
| 6 | Lich su kham benh | Xem toan bo lich su kham |
| 7 | Xem don thuoc | Xem don thuoc da ke |
| 8 | Nhac uong thuoc | Thong bao nhac gio uong thuoc |
| 9 | Thanh toan online | Thanh toan vien phi qua app |
| 10 | Lich su thanh toan | Xem hoa don, bien lai |
| 11 | Nhan tin bac si | Chat voi bac si dieu tri |
| 12 | Upload tai lieu | Gui file, anh cho bac si |
| 13 | Tom tat suc khoe | Tong quan suc khoe ca nhan |
| 14 | Truy cap thanh vien gia dinh | Quan ly ho so nguoi than |
| 15 | Gop y/khao sat | Danh gia chat luong dich vu |
| 16 | Cai dat thong bao | Tuy chon nhan thong bao |
| 17 | Kien thuc suc khoe | Bai viet giao duc suc khoe |
| 18 | So tiem chung | Xem lich su tiem vaccine |
| 19 | Trang thai chuyen vien | Theo doi tinh trang giay chuyen tuyen |
| 20 | Dong bo thiet bi deo | Ket noi smartwatch, fitness tracker |
| 21 | Lien he khan cap | Cap nhat thong tin lien he khan cap |
| 22 | Quan ly dong y | Xem va ky consent form online |
| 23 | Xuat du lieu (FHIR) | Tai ho so suc khoe theo chuan FHIR |
| 24 | Push notification | Thong bao lich hen, ket qua, nhac thuoc |
| 25 | Chatbot ho tro | Tro ly ao tra loi cau hoi thuong gap |

---

## 13. Tich hop & Lien thong

> **25 features** — HL7, FHIR, BHXH, SSO, webhook

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | HL7 v2 messaging | Gui/nhan thong diep HL7 v2.x |
| 2 | HL7 FHIR R4 API | RESTful API theo chuan FHIR R4 |
| 3 | Tich hop LIS | Ket noi he thong xet nghiem |
| 4 | Tich hop PACS/RIS | Ket noi he thong CDHA |
| 5 | DICOM gateway | Cong tiep nhan anh DICOM |
| 6 | Cong BHXH (XML 4210) | Gui du lieu giam dinh BHXH |
| 7 | Cong bao cao CDC | Bao cao benh truyen nhiem len CDC |
| 8 | Tich hop he thong duoc | Ket noi DMS, nha thuoc ngoai |
| 9 | Tich hop cong bao hiem | Tra cuu, gui claim bao hiem |
| 10 | Tich hop cong thanh toan | VNPay, Momo, ngan hang |
| 11 | Tich hop SMS gateway | Gui SMS tu dong |
| 12 | Tich hop email | Gui email thong bao, bao cao |
| 13 | Single Sign-On (SSO) | Dang nhap mot lan (Keycloak, Azure AD) |
| 14 | Tich hop nha cung cap dinh danh | LDAP, SAML, OpenID Connect |
| 15 | Master Patient Index | Dinh danh benh nhan toan he thong |
| 16 | Health Information Exchange | Trao doi du lieu giua co so y te |
| 17 | Tich hop thiet bi IoT | Ket noi thiet bi deo, cam bien |
| 18 | API cho ung dung thu ba | Open API cho partner tich hop |
| 19 | Cong cu nhap/chuyen doi du lieu | Import tu he thong cu |
| 20 | Xuat du lieu | Export CSV, Excel, PDF |
| 21 | He thong webhook | Event-driven thong bao realtime |
| 22 | Rate limiting & monitoring | Kiem soat luu luong API |
| 23 | Xu ly loi & tu dong thu lai | Retry mechanism cho tich hop |
| 24 | Nhat ky tich hop | Audit log moi giao dich lien thong |
| 25 | FHIR Bulk Data Export | Xuat du lieu lon theo chuan FHIR Bulk |

---

## 14. Dieu duong & Quan ly buong

> **25 features** — Giuong benh, dieu duong, ban giao ca, MAR

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Quan ly giuong benh | Cai dat giuong theo khoa, phong, buong |
| 2 | Dashboard giuong trong | Hien thi real-time giuong con trong |
| 3 | Phan giuong | Xep giuong cho benh nhan nhap vien |
| 4 | Chuyen giuong | Chuyen benh nhan giua cac giuong/phong |
| 5 | Thong ke buong benh | Census — so benh nhan dang nam vien |
| 6 | Phieu danh gia dieu duong | Form danh gia cua dieu duong |
| 7 | Ke hoach cham soc | Nursing care plan cho tung benh nhan |
| 8 | Phieu theo doi thuoc (MAR) | Medication Administration Record |
| 9 | Bieu do sinh hieu | Charting: nhiet do, mach, HA, SpO2 |
| 10 | Theo doi vao/ra | Intake/output: dich truyen, nuoc tieu |
| 11 | Danh gia nguy co te nga | Fall risk assessment scoring |
| 12 | Danh gia dau | Pain assessment scale |
| 13 | Ghi nhan cham soc vet thuong | Wound care documentation |
| 14 | Phieu ban giao benh nhan | Handoff report khi chuyen ca |
| 15 | Ban giao ca truc | Shift handover — dieu duong giao ca |
| 16 | Quan ly cong viec dieu duong | Task list cho tung ca truc |
| 17 | Lich di buong | Patient rounding schedule |
| 18 | Canh bao cach ly | Alert benh nhan can cach ly |
| 19 | In vong tay benh nhan | In wristband dinh danh |
| 20 | Dashboard khoi luong cong viec | Workload cua tung dieu duong |
| 21 | Ke hoach xuat vien | Discharge planning va huong dan |
| 22 | Giao duc benh nhan | Tai lieu huong dan cham soc |
| 23 | KPI dieu duong | Chi so hieu suat dieu duong |
| 24 | Ghi chu dieu duong | Nurse note theo doi hang ngay |
| 25 | Phan tich buong benh | Thong ke cong suat, thoi gian nam |

---

## 15. Phong mo & Phau thuat

> **20 features** — Lich mo, WHO checklist, gay me, hoi suc

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Xep lich phau thuat | Dat lich mo cho benh nhan |
| 2 | Lich phong mo | Calendar phong mo theo ngay |
| 3 | Quan ly phong mo | Tinh trang phong mo: trong, dang su dung |
| 4 | Danh gia tien phau | Kham va danh gia truoc mo |
| 5 | Checklist phau thuat (WHO) | WHO Surgical Safety Checklist |
| 6 | Phieu gay me | Ghi nhan quy trinh gay me/hoi suc |
| 7 | Ghi nhan trong mo | Intra-operative note |
| 8 | Ghi nhan sau mo | Post-operative note |
| 9 | Theo doi dung cu phau thuat | Kiem dem dung cu truoc/sau mo |
| 10 | Phieu dong y phau thuat | Consent form phau thuat |
| 11 | Phan cong ekip mo | Phan cong phau thuat vien, gay me, dieu duong |
| 12 | Thoi gian phau thuat | Theo doi thoi gian tung giai doan mo |
| 13 | Bien chung phau thuat | Ghi nhan va theo doi bien chung |
| 14 | Thanh toan phau thuat | Chi phi phau thuat, vat tu, gay me |
| 15 | Bao cao phau thuat | Bao cao ket qua phau thuat |
| 16 | Phan tich su dung phong mo | OR utilization analytics |
| 17 | Theo doi huy mo | Ghi nhan ly do huy/hoan phau thuat |
| 18 | Quan ly vat tu phau thuat | Vat tu tieu hao trong mo |
| 19 | Quan ly phong hoi suc | Recovery room sau phau thuat |
| 20 | Nhat ky phau thuat | Audit log moi thao tac |

---

## 16. Tuan thu & Bao mat

> **20 features** — RBAC, MFA, ma hoa, DPIA, kiem soat truy cap

| # | Feature | Mo ta |
|---|---------|-------|
| 1 | Kiem soat truy cap (RBAC) | Phan quyen theo vai tro |
| 2 | Xac thuc da yeu to (MFA) | OTP, authenticator app, SMS |
| 3 | Ma hoa du lieu luu tru | AES-256 encryption at rest |
| 4 | Ma hoa du lieu truyen tai | TLS 1.3 encryption in transit |
| 5 | Nhat ky bat bien | Immutable audit trail |
| 6 | Quan ly dong y | Consent management theo quy dinh |
| 7 | Chinh sach luu tru du lieu | Data retention policy cau hinh |
| 8 | An danh hoa du lieu | De-identification cho nghien cuu |
| 9 | Gia danh hoa du lieu | Pseudonymization cho phan tich |
| 10 | Quy trinh thong bao vi pham | Breach notification workflow |
| 11 | Danh gia tac dong DPIA | Data Protection Impact Assessment |
| 12 | Dashboard tuan thu | Tong quan trang thai tuan thu |
| 13 | Tao bao cao tuan thu | Bao cao gui co quan quan ly |
| 14 | Xu ly yeu cau truy cap du lieu | Data access request handling |
| 15 | Quy trinh xoa du lieu | Right to erasure workflow |
| 16 | Luu tru du lieu noi dia | Data localization enforcement |
| 17 | Quan ly phien & timeout | Session management bao mat |
| 18 | IP whitelist/blacklist | Han che truy cap theo IP |
| 19 | Nhat ky su co bao mat | Security incident logging |
| 20 | Theo doi pentest | Penetration test report tracking |

---

> **Tong cong: 400 features** tren 16 modules, bao phu toan bo quy trinh van hanh benh vien va phong kham theo tieu chuan quoc te.
