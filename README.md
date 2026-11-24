# happyhoof-media

Kho hình + audio cho **Flashcard** và **Self-study Room** của Happy Hoof English (tách khỏi repo chính để repo chính không phình).

```
flashcards/img/    hình thẻ         flashcards/audio/  audio từ + câu ví dụ
study/img/         hình slide       study/audio/       audio slide
```

## Quy ước đặt tên
- Chữ thường, không dấu, nối bằng gạch dưới: `family_friends_a1_mother.webp`, `animals_a2_giraffe_ex1.m4a`.
- Không dùng khoảng trắng. **Đã đăng lên thì không đổi tên** (app nhớ theo tên). Trình duyệt giữ bản cũ tối đa 1 ngày (`_headers`), nên ghi đè cùng tên thì HS thấy bản mới sau ≤ 1 ngày.

## Định dạng
- Hình thẻ Flashcard: **SVG 400×400 (~2–8 KB)** cho biểu tượng Twemoji; **WebP 400×400 (~20 KB)** cho hình vẽ AI (khi không có biểu tượng đúng nghĩa). Từ trừu tượng không có hình. Hình slide: **WebP 640×400, ~30 KB**.
- Audio câu ngắn: **m4a mono 48 kbps**.

## Địa chỉ
`https://happyhoof-media.pages.dev/flashcards/img/mau_ngua.webp` (file mẫu, xóa được sau).
App đọc qua `mediaUrl()` trong `src/lib/media.ts` của repo chính.

## Nguồn hình + giấy phép
- **Twemoji** © X Corp & contributors — giấy phép **CC-BY 4.0** (https://creativecommons.org/licenses/by/4.0/), nguồn https://github.com/jdecked/twemoji (bản 15.1.0). Dùng trong nhiều hình `flashcards/img/**/*.svg` (có ghép, thêm nền). Ghi công trong app: chân màn Flashcards.
- Hình vẽ AI trên máy (Animagine XL 4.0, giấy phép openrail++): của Happy Hoof English.
- Audio: giọng máy Kokoro-82M (Apache 2.0) chạy trên máy.
