# happyhoof-media

Kho hình + audio cho **Flashcard** và **Self-study Room** của Happy Hoof English (tách khỏi repo chính để repo chính không phình).

```
flashcards/img/    hình thẻ         flashcards/audio/  audio từ + câu ví dụ
study/img/         hình slide       study/audio/       audio slide
```

## Quy ước đặt tên
- Chữ thường, không dấu, nối bằng gạch dưới: `family_friends_a1_mother.webp`, `animals_a2_giraffe_ex1.m4a`.
- Không dùng khoảng trắng. **Đã đăng lên thì không đổi tên** (app nhớ theo tên; cache 1 năm). Muốn đổi hình: đặt tên mới.

## Định dạng
- Hình thẻ: **WebP 400×400, ~20 KB**. Hình slide: **WebP 640×400, ~30 KB**.
- Audio câu ngắn: **m4a mono 48 kbps**.

## Địa chỉ
`https://happyhoof-media.pages.dev/flashcards/img/mau_ngua.webp` (file mẫu, xóa được sau).
App đọc qua `mediaUrl()` trong `src/lib/media.ts` của repo chính.
