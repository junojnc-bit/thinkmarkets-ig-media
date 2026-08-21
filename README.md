# thinkmarkets-ig-media

公開素材託管，給 Instagram Content Publishing API 抓影片/圖片用。

IG 的 Content Publishing API（`{ig-user-id}/media`）只接受**匿名可抓取的公開 HTTPS 網址**
作為 `video_url` / `image_url`，不接受檔案上傳或私有連結。`thinkmarkets-tw` 是私有 repo，
GitHub Release 的下載連結在私有 repo 裡對匿名請求會回 404（已實測），所以另開這個
專門託管用的公開 repo，不放任何程式碼。

用法見 `thinkmarkets-tw` 的 `data/ig-publish/host-asset.mjs`。

素材發布成功後可以刪掉對應的 release asset，不用長期保留——IG 收到之後
會存進自己的 CDN，這裡的檔案只是「送過去」用的暫時中繼站。
