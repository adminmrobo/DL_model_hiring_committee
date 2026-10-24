# 모델 채용 위원회 2차 공채 — 딥러닝 열다섯 명의 입사 면접

콘크리트 공장의 두 번째 공채입니다. 지원자는 퍼셉트론부터 확산 모델까지 신경망 열다섯 명이고, 합격하려면 1차 공채로 뽑은 선배(KNN · SVM · GBM · GMM · PCA 등)보다 같은 조건에서 나아야 합니다. 판정은 Colab(PyTorch)에서 씨앗 다섯 개로 실제로 학습한 평균이며, 보류된 지원자는 미리 등록한 조건으로 한 번 재시험을 청할 수 있습니다. 결과: 합격 3명(재시험 합격 1명 포함), 보류 12명 — "딥러닝이 늘 이기지는 않는다".

- 글: 안상선 ((주)M-Robo 대표)
- 라이선스: CC BY-NC 4.0 (비상업적 이용, 출처 표기 필수) — [LICENSE.md](LICENSE.md)
- 시작: [index.html](index.html)

## 언어 / Languages

모든 페이지를 영어·중국어·일본어·러시아어·우즈베크어·베트남어로도 볼 수 있습니다. 위쪽 메뉴의 언어 선택 상자로 바꾸고, 처음 방문하면 브라우저 언어에 맞는 판으로 자동으로 이동합니다(고른 언어는 기억). 주소 뒤에 ?lang=en 처럼 붙여 직접 지정할 수도 있습니다. Colab 코드와 실행 결과는 한국어 원문 그대로입니다.

| 언어 | 폴더 |
|---|---|
| 한국어 (기본) | / |
| English | en/ |
| 中文 (简体) | zh/ |
| 日本語 | ja/ |
| Русский | ru/ |
| Oʻzbekcha | uz/ |
| Tiếng Việt | vi/ |

## 편 목록

6-0 2차 채용 공고(딥러닝 치트시트)에서 전체 지도를 보고, 각 편이 끝나면 다시 6-0으로 돌아옵니다.

| 편 | 파일 | 제목 | 팀 | 판정 |
|---|---|---|---|---|
| 6-0 | [6-0_job_posting.html](6-0_job_posting.html) | 2차 채용 공고 · 딥러닝 치트시트 | 채용 공고 |  |
| 6-1 | [6-1_perceptron.html](6-1_perceptron.html) | 퍼셉트론 | 표 데이터팀 | 재시험 합격 |
| 6-2 | [6-2_mlp.html](6-2_mlp.html) | 다층 퍼셉트론 | 표 데이터팀 | 보류 확정 |
| 6-3 | [6-3_resnet.html](6-3_resnet.html) | ResNet | 표 데이터팀 | 보류 |
| 6-4 | [6-4_cnn.html](6-4_cnn.html) | CNN | 이미지팀 | 보류 확정 |
| 6-5 | [6-5_siamese.html](6-5_siamese.html) | 샴 네트워크 | 이미지팀 | 보류 확정 |
| 6-6 | [6-6_rnn.html](6-6_rnn.html) | RNN | 순서팀 | 보류 |
| 6-7 | [6-7_lstm.html](6-7_lstm.html) | LSTM | 순서팀 | 보류 확정 |
| 6-8 | [6-8_gru.html](6-8_gru.html) | GRU | 순서팀 | 보류 확정 |
| 6-9 | [6-9_transformer.html](6-9_transformer.html) | Transformer | 주의팀 | 보류 확정 |
| 6-10 | [6-10_som.html](6-10_som.html) | SOM | 군집팀 | 보류 |
| 6-11 | [6-11_autoencoder.html](6-11_autoencoder.html) | 오토인코더 | 압축팀 | 합격 |
| 6-12 | [6-12_denoising_ae.html](6-12_denoising_ae.html) | 디노이징 오토인코더 | 압축팀 | 합격 |
| 6-13 | [6-13_vae.html](6-13_vae.html) | VAE | 생성팀 | 보류 |
| 6-14 | [6-14_gan.html](6-14_gan.html) | GAN | 생성팀 | 보류 |
| 6-15 | [6-15_diffusion.html](6-15_diffusion.html) | 확산 모델 | 생성팀 | 보류 확정 |

## 각 편에 들어 있는 것

- 지원서 1장 — 한 장 요약
- 면접 장면, 브라우저에서 직접 학습해 보는 실습과 움직이는 그림, 확인 문제
- 재시험(이의 신청) — 지원자가 근거를 대고 사전 등록한 조건으로 다시 시험
- Colab 코드(PyTorch) — 복사, .py · .ipynb 내려받기. 페이지에 실제 실행 결과를 실었습니다
- AI 비서 코드의 실수 찾기, AI 응용 프롬프트, 용어 정리, 비유 모음, 레퍼런스
- 교육자를 위한 TIP

## 데이터

- 표 데이터팀(6-1 ~ 6-3): UCI Machine Learning Repository, Concrete Compressive Strength (Yeh, 1998, 1,030건, CC BY 4.0)
- 그 밖의 편(6-4 ~ 6-15): scikit-learn 내장 손글씨 숫자 load_digits (1,797장)

각 HTML은 그림·데이터·스크립트를 파일 안에 담고 있어 빌드 없이 브라우저로 열면 됩니다(글꼴만 Google Fonts에서 불러옵니다). 편끼리의 링크는 같은 폴더 구조에서 작동하므로 파일 이름을 바꾸지 마세요. 1차 공채(머신러닝 편)는 별도 저장소입니다.

---

# The Model Hiring Committee, Second Open Recruitment — Fifteen Deep-Learning Candidates

The concrete plant opens its second recruitment. The candidates are fifteen neural networks, from the perceptron to the diffusion model, and to be hired each must beat a senior hired in the first recruitment (KNN, SVM, GBM, GMM, PCA and others) under the same conditions. Verdicts use the mean of five seeds actually trained in Colab (PyTorch), and a candidate put on hold may appeal once for a retest under pre-registered conditions. Result: 3 hired (1 on retest), 12 on hold — "deep learning does not always win".

- Author: Ahn Sangsun (CEO, M-Robo Co., Ltd.)
- License: CC BY-NC 4.0 (non-commercial use, attribution required) — [LICENSE.md](LICENSE.md)
- Start: [en/index.html](en/index.html)

## Episodes

Start with the full map in 6-0 (job posting and deep-learning cheat sheet); every episode leads back to it.

| Ep. | File | Title | Team | Verdict |
|---|---|---|---|---|
| 6-0 | [en/6-0_job_posting.html](en/6-0_job_posting.html) | Second recruitment notice · Deep learning cheat sheet | Job posting |  |
| 6-1 | [en/6-1_perceptron.html](en/6-1_perceptron.html) | Perceptron | Tabular Data Team | Hired on retest |
| 6-2 | [en/6-2_mlp.html](en/6-2_mlp.html) | Multilayer perceptron | Tabular Data Team | On hold (final) |
| 6-3 | [en/6-3_resnet.html](en/6-3_resnet.html) | ResNet | Tabular Data Team | On hold |
| 6-4 | [en/6-4_cnn.html](en/6-4_cnn.html) | CNN | Image Team | On hold (final) |
| 6-5 | [en/6-5_siamese.html](en/6-5_siamese.html) | Siamese network | Image Team | On hold (final) |
| 6-6 | [en/6-6_rnn.html](en/6-6_rnn.html) | RNN | Sequence Team | On hold |
| 6-7 | [en/6-7_lstm.html](en/6-7_lstm.html) | LSTM | Sequence Team | On hold (final) |
| 6-8 | [en/6-8_gru.html](en/6-8_gru.html) | GRU | Sequence Team | On hold (final) |
| 6-9 | [en/6-9_transformer.html](en/6-9_transformer.html) | Transformer | Attention Team | On hold (final) |
| 6-10 | [en/6-10_som.html](en/6-10_som.html) | SOM | Clustering Team | On hold |
| 6-11 | [en/6-11_autoencoder.html](en/6-11_autoencoder.html) | Autoencoder | Compression Team | Hired |
| 6-12 | [en/6-12_denoising_ae.html](en/6-12_denoising_ae.html) | Denoising autoencoder | Compression Team | Hired |
| 6-13 | [en/6-13_vae.html](en/6-13_vae.html) | VAE | Generation Team | On hold |
| 6-14 | [en/6-14_gan.html](en/6-14_gan.html) | GAN | Generation Team | On hold |
| 6-15 | [en/6-15_diffusion.html](en/6-15_diffusion.html) | Diffusion model | Generation Team | On hold (final) |

## In every episode

- Application, page 1 — a one-page overview
- Interview scenes, labs you train in the browser, animated diagrams, check questions
- Retest (appeal) — the candidate argues its case and is retested under pre-registered conditions
- Colab code (PyTorch) — copy, download .py / .ipynb; real run output is shown on the page
- Bug hunt in AI-assistant code, AI prompts, glossary, analogies, references
- Tips for educators

## Data

- Tabular Data Team (6-1 – 6-3): UCI Machine Learning Repository, Concrete Compressive Strength (Yeh, 1998, 1,030 mixes, CC BY 4.0)
- Other episodes (6-4 – 6-15): scikit-learn built-in handwritten digits, load_digits (1,797 images)

Each HTML file contains its images, data and scripts, so you just open it in a browser (only fonts load from Google Fonts). Links between episodes work in the same folder layout, so keep the file names. The First Open Recruitment (machine learning) is a separate repository.

---

# 模型招聘委员会 第二次公开招聘 — 十五位深度学习应聘者的入职面试

混凝土工厂开启第二次招聘。应聘者是从感知机到扩散模型的十五个神经网络；要被录用，必须在相同条件下胜过第一次招聘录用的前辈（KNN、SVM、GBM、GMM、PCA 等）。判定采用在 Colab（PyTorch）中用五个随机种子实际训练的平均值；被判待定的应聘者可按事先登记的条件申请一次复试。结果：录用 3 人（含复试录用 1 人），待定 12 人——“深度学习并不总是赢”。

- 作者：Ahn Sangsun（M-Robo 公司代表）
- 许可：CC BY-NC 4.0（非商业使用，须注明出处） — [LICENSE.md](LICENSE.md)
- 开始: [zh/index.html](zh/index.html)

## 篇章目录

先在 6-0 第二次招聘启事（深度学习速查表）看全图，每一篇结束后都会回到 6-0。

| 篇 | 文件 | 标题 | 小组 | 判定 |
|---|---|---|---|---|
| 6-0 | [zh/6-0_job_posting.html](zh/6-0_job_posting.html) | 第二次招聘启事 · 深度学习速查表 | 招聘启事 |  |
| 6-1 | [zh/6-1_perceptron.html](zh/6-1_perceptron.html) | 感知机 | 表格数据组 | 复试录用 |
| 6-2 | [zh/6-2_mlp.html](zh/6-2_mlp.html) | 多层感知机 | 表格数据组 | 待定（最终） |
| 6-3 | [zh/6-3_resnet.html](zh/6-3_resnet.html) | ResNet | 表格数据组 | 待定 |
| 6-4 | [zh/6-4_cnn.html](zh/6-4_cnn.html) | CNN | 图像组 | 待定（最终） |
| 6-5 | [zh/6-5_siamese.html](zh/6-5_siamese.html) | 孪生网络 | 图像组 | 待定（最终） |
| 6-6 | [zh/6-6_rnn.html](zh/6-6_rnn.html) | RNN | 序列组 | 待定 |
| 6-7 | [zh/6-7_lstm.html](zh/6-7_lstm.html) | LSTM | 序列组 | 待定（最终） |
| 6-8 | [zh/6-8_gru.html](zh/6-8_gru.html) | GRU | 序列组 | 待定（最终） |
| 6-9 | [zh/6-9_transformer.html](zh/6-9_transformer.html) | Transformer | 注意力组 | 待定（最终） |
| 6-10 | [zh/6-10_som.html](zh/6-10_som.html) | SOM | 聚类组 | 待定 |
| 6-11 | [zh/6-11_autoencoder.html](zh/6-11_autoencoder.html) | 自编码器 | 压缩组 | 录用 |
| 6-12 | [zh/6-12_denoising_ae.html](zh/6-12_denoising_ae.html) | 去噪自编码器 | 压缩组 | 录用 |
| 6-13 | [zh/6-13_vae.html](zh/6-13_vae.html) | VAE | 生成组 | 待定 |
| 6-14 | [zh/6-14_gan.html](zh/6-14_gan.html) | GAN | 生成组 | 待定 |
| 6-15 | [zh/6-15_diffusion.html](zh/6-15_diffusion.html) | 扩散模型 | 生成组 | 待定（最终） |

## 每篇包含

- 申请表·第1页 — 一页总览
- 面试场景、在浏览器中亲手训练的实验与动态图示、确认题
- 复试（申诉）— 应聘者陈述理由，按事先登记的条件重新考试
- Colab 代码（PyTorch）— 可复制、下载 .py / .ipynb，页面附有真实运行结果
- 找出 AI 助手代码中的错误、AI 应用提示词、术语表、比喻集、参考文献
- 给教育者的 TIP

## 数据

- 表格数据组（6-1 ~ 6-3）：UCI Machine Learning Repository，Concrete Compressive Strength（Yeh, 1998，1,030 组，CC BY 4.0）
- 其他篇（6-4 ~ 6-15）：scikit-learn 内置手写数字 load_digits（1,797 张）

每个 HTML 文件都内含图片、数据和脚本，用浏览器直接打开即可（只有字体从 Google Fonts 加载）。篇与篇之间的链接依赖相同的文件夹结构，请勿更改文件名。第一次公开招聘（机器学习篇）在另一个仓库。

---

# モデル採用委員会 第2次公募 — ディープラーニング15名の入社面接

コンクリート工場の2回目の公募です。応募者はパーセプトロンから拡散モデルまでのニューラルネットワーク15名。採用されるには、第1次公募で採用された先輩（KNN・SVM・GBM・GMM・PCA など）に同じ条件で勝たなければなりません。判定は Colab（PyTorch）で5つのシードで実際に学習した平均で、保留になった応募者は事前登録した条件で一度だけ再試験を求められます。結果：採用3名（再試験での採用1名を含む）、保留12名——「ディープラーニングがいつも勝つわけではない」。

- 著者：アン・サンソン（株式会社 M-Robo 代表）
- ライセンス：CC BY-NC 4.0（非営利利用、出典表示必須） — [LICENSE.md](LICENSE.md)
- スタート: [ja/index.html](ja/index.html)

## 編の一覧

まず 6-0 第2次求人票（ディープラーニング・チートシート）で全体マップを見てください。各編の最後は 6-0 に戻ります。

| 編 | ファイル | タイトル | チーム | 判定 |
|---|---|---|---|---|
| 6-0 | [ja/6-0_job_posting.html](ja/6-0_job_posting.html) | 第2次求人票 · ディープラーニング・チートシート | 求人票 |  |
| 6-1 | [ja/6-1_perceptron.html](ja/6-1_perceptron.html) | パーセプトロン | 表データチーム | 再試験で採用 |
| 6-2 | [ja/6-2_mlp.html](ja/6-2_mlp.html) | 多層パーセプトロン | 表データチーム | 保留（確定） |
| 6-3 | [ja/6-3_resnet.html](ja/6-3_resnet.html) | ResNet | 表データチーム | 保留 |
| 6-4 | [ja/6-4_cnn.html](ja/6-4_cnn.html) | CNN | 画像チーム | 保留（確定） |
| 6-5 | [ja/6-5_siamese.html](ja/6-5_siamese.html) | シャムネットワーク | 画像チーム | 保留（確定） |
| 6-6 | [ja/6-6_rnn.html](ja/6-6_rnn.html) | RNN | 系列チーム | 保留 |
| 6-7 | [ja/6-7_lstm.html](ja/6-7_lstm.html) | LSTM | 系列チーム | 保留（確定） |
| 6-8 | [ja/6-8_gru.html](ja/6-8_gru.html) | GRU | 系列チーム | 保留（確定） |
| 6-9 | [ja/6-9_transformer.html](ja/6-9_transformer.html) | Transformer | アテンションチーム | 保留（確定） |
| 6-10 | [ja/6-10_som.html](ja/6-10_som.html) | SOM | クラスタリングチーム | 保留 |
| 6-11 | [ja/6-11_autoencoder.html](ja/6-11_autoencoder.html) | オートエンコーダ | 圧縮チーム | 採用 |
| 6-12 | [ja/6-12_denoising_ae.html](ja/6-12_denoising_ae.html) | デノイジング・オートエンコーダ | 圧縮チーム | 採用 |
| 6-13 | [ja/6-13_vae.html](ja/6-13_vae.html) | VAE | 生成チーム | 保留 |
| 6-14 | [ja/6-14_gan.html](ja/6-14_gan.html) | GAN | 生成チーム | 保留 |
| 6-15 | [ja/6-15_diffusion.html](ja/6-15_diffusion.html) | 拡散モデル | 生成チーム | 保留（確定） |

## 各編の内容

- 応募書類・1枚目 — 1枚まとめ
- 面接シーン、ブラウザで実際に学習させる実習と動く図、確認問題
- 再試験（異議申し立て）— 応募者が根拠を示し、事前登録した条件で再試験
- Colab コード（PyTorch）— コピー、.py / .ipynb のダウンロード。実際の実行結果をページに掲載
- AI アシスタントのコードの誤り探し、AI 活用プロンプト、用語集、たとえ集、参考文献
- 教育者向け TIP

## データ

- 表データチーム（6-1 〜 6-3）：UCI Machine Learning Repository, Concrete Compressive Strength（Yeh, 1998, 1,030件, CC BY 4.0）
- その他の編（6-4 〜 6-15）：scikit-learn 内蔵の手書き数字 load_digits（1,797枚）

各 HTML は画像・データ・スクリプトをファイル内に持っているので、ビルドなしでブラウザで開くだけです（フォントのみ Google Fonts から読み込みます）。編どうしのリンクは同じフォルダ構成で動くので、ファイル名は変えないでください。第1次公募（機械学習編）は別のリポジトリです。

---

# Modellarni ishga olish qoʻmitasi, Ikkinchi ochiq tanlov — oʻn besh chuqur oʻqitish nomzodining suhbati

Beton zavodi ikkinchi tanlovni eʼlon qiladi. Nomzodlar — perseptrondan diffuziya modeligacha boʻlgan oʻn beshta neyron tarmoq; ishga olinish uchun har biri bir xil sharoitda birinchi tanlovda olingan katta hamkasbdan (KNN, SVM, GBM, GMM, PCA va boshqalar) ustun kelishi kerak. Qaror Colab (PyTorch) da beshta seed bilan haqiqatda oʻqitilgan oʻrtacha natijaga asoslanadi; kutishga qoldirilgan nomzod oldindan roʻyxatga olingan shartlar bilan bir marta qayta sinov soʻrashi mumkin. Natija: 3 nafar ishga olindi (1 nafari qayta sinovda), 12 nafar kutishda — «chuqur oʻqitish har doim ham yutmaydi».

- Muallif: Ahn Sangsun (M-Robo kompaniyasi rahbari)
- Litsenziya: CC BY-NC 4.0 (notijorat foydalanish, manbani koʻrsatish majburiy) — [LICENSE.md](LICENSE.md)
- Boshlash: [uz/index.html](uz/index.html)

## Boblar

Avval 6-0 (ikkinchi vakansiya eʼloni va chuqur oʻqitish shpargalkasi) da umumiy xaritani koʻring; har bir bob oxirida yana 6-0 ga qaytasiz.

| Bob | Fayl | Sarlavha | Jamoa | Qaror |
|---|---|---|---|---|
| 6-0 | [uz/6-0_job_posting.html](uz/6-0_job_posting.html) | Ikkinchi tanlov eʼloni · Chuqur oʻqitish shpargalkasi | Vakansiya eʼloni |  |
| 6-1 | [uz/6-1_perceptron.html](uz/6-1_perceptron.html) | Perseptron | Jadval maʼlumotlari jamoasi | Qayta sinovda olindi |
| 6-2 | [uz/6-2_mlp.html](uz/6-2_mlp.html) | Koʻp qatlamli perseptron | Jadval maʼlumotlari jamoasi | Kutishda (yakuniy) |
| 6-3 | [uz/6-3_resnet.html](uz/6-3_resnet.html) | ResNet | Jadval maʼlumotlari jamoasi | Kutishda |
| 6-4 | [uz/6-4_cnn.html](uz/6-4_cnn.html) | CNN | Tasvir jamoasi | Kutishda (yakuniy) |
| 6-5 | [uz/6-5_siamese.html](uz/6-5_siamese.html) | Siam tarmogʻi | Tasvir jamoasi | Kutishda (yakuniy) |
| 6-6 | [uz/6-6_rnn.html](uz/6-6_rnn.html) | RNN | Ketma-ketlik jamoasi | Kutishda |
| 6-7 | [uz/6-7_lstm.html](uz/6-7_lstm.html) | LSTM | Ketma-ketlik jamoasi | Kutishda (yakuniy) |
| 6-8 | [uz/6-8_gru.html](uz/6-8_gru.html) | GRU | Ketma-ketlik jamoasi | Kutishda (yakuniy) |
| 6-9 | [uz/6-9_transformer.html](uz/6-9_transformer.html) | Transformer | Diqqat jamoasi | Kutishda (yakuniy) |
| 6-10 | [uz/6-10_som.html](uz/6-10_som.html) | SOM | Klasterlash jamoasi | Kutishda |
| 6-11 | [uz/6-11_autoencoder.html](uz/6-11_autoencoder.html) | Avtoenkoder | Siqish jamoasi | Olindi |
| 6-12 | [uz/6-12_denoising_ae.html](uz/6-12_denoising_ae.html) | Denoising avtoenkoder | Siqish jamoasi | Olindi |
| 6-13 | [uz/6-13_vae.html](uz/6-13_vae.html) | VAE | Generatsiya jamoasi | Kutishda |
| 6-14 | [uz/6-14_gan.html](uz/6-14_gan.html) | GAN | Generatsiya jamoasi | Kutishda |
| 6-15 | [uz/6-15_diffusion.html](uz/6-15_diffusion.html) | Diffuziya modeli | Generatsiya jamoasi | Kutishda (yakuniy) |

## Har bir bobda

- Ariza, 1-sahifa — bir sahifalik xulosa
- Suhbat sahnalari, brauzerda oʻzingiz oʻqitadigan mashqlar va harakatlanuvchi rasmlar, tekshiruv savollari
- Qayta sinov (eʼtiroz) — nomzod dalil keltiradi va oldindan roʻyxatga olingan shartlar bilan qayta sinaladi
- Colab kodi (PyTorch) — nusxa olish, .py / .ipynb yuklab olish; sahifada haqiqiy natija koʻrsatilgan
- AI yordamchi kodidagi xatolarni topish, AI uchun promptlar, atamalar lugʻati, oʻxshatishlar, manbalar
- Oʻqituvchilar uchun maslahatlar

## Maʼlumotlar

- Jadval maʼlumotlari jamoasi (6-1 – 6-3): UCI Machine Learning Repository, Concrete Compressive Strength (Yeh, 1998, 1,030 ta tarkib, CC BY 4.0)
- Boshqa boblar (6-4 – 6-15): scikit-learn ichidagi qoʻlyozma raqamlar load_digits (1,797 ta rasm)

Har bir HTML fayl rasmlar, maʼlumotlar va skriptlarni oʻz ichida saqlaydi — brauzerda ochish kifoya (faqat shriftlar Google Fonts dan yuklanadi). Boblar orasidagi havolalar bir xil papka tuzilmasida ishlaydi, shuning uchun fayl nomlarini oʻzgartirmang. Birinchi ochiq tanlov (mashinali oʻqitish) alohida repozitoriyda.

---

# Комиссия по найму моделей, Второй открытый набор — собеседование пятнадцати кандидатов глубокого обучения

Бетонный завод объявляет второй набор. Кандидаты — пятнадцать нейросетей, от перцептрона до диффузионной модели; чтобы получить работу, каждая должна в тех же условиях превзойти старшего сотрудника из первого набора (KNN, SVM, GBM, GMM, PCA и др.). Решение принимается по среднему пяти сидов, реально обученных в Colab (PyTorch); отложенный кандидат может один раз подать апелляцию на пересдачу по заранее зарегистрированным условиям. Итог: принято 3 (из них 1 после пересдачи), отложено 12 — «глубокое обучение побеждает не всегда».

- Автор: Ан Сансон (генеральный директор M-Robo Co., Ltd.)
- Лицензия: CC BY-NC 4.0 (некоммерческое использование, обязательное указание авторства) — [LICENSE.md](LICENSE.md)
- Начать: [ru/index.html](ru/index.html)

## Главы

Начните с общей карты в 6-0 (объявление о втором наборе и шпаргалка по глубокому обучению); каждая глава возвращает к ней.

| Глава | Файл | Название | Группа | Решение |
|---|---|---|---|---|
| 6-0 | [ru/6-0_job_posting.html](ru/6-0_job_posting.html) | Объявление о Втором наборе · Шпаргалка по глубокому обучению | Объявление |  |
| 6-1 | [ru/6-1_perceptron.html](ru/6-1_perceptron.html) | Перцептрон | Группа табличных данных | Принято после пересдачи |
| 6-2 | [ru/6-2_mlp.html](ru/6-2_mlp.html) | Многослойный перцептрон | Группа табличных данных | Отложено (окончательно) |
| 6-3 | [ru/6-3_resnet.html](ru/6-3_resnet.html) | ResNet | Группа табличных данных | Отложено |
| 6-4 | [ru/6-4_cnn.html](ru/6-4_cnn.html) | CNN | Группа изображений | Отложено (окончательно) |
| 6-5 | [ru/6-5_siamese.html](ru/6-5_siamese.html) | Сиамская сеть | Группа изображений | Отложено (окончательно) |
| 6-6 | [ru/6-6_rnn.html](ru/6-6_rnn.html) | RNN | Группа последовательностей | Отложено |
| 6-7 | [ru/6-7_lstm.html](ru/6-7_lstm.html) | LSTM | Группа последовательностей | Отложено (окончательно) |
| 6-8 | [ru/6-8_gru.html](ru/6-8_gru.html) | GRU | Группа последовательностей | Отложено (окончательно) |
| 6-9 | [ru/6-9_transformer.html](ru/6-9_transformer.html) | Transformer | Группа внимания | Отложено (окончательно) |
| 6-10 | [ru/6-10_som.html](ru/6-10_som.html) | SOM | Группа кластеризации | Отложено |
| 6-11 | [ru/6-11_autoencoder.html](ru/6-11_autoencoder.html) | Автоэнкодер | Группа сжатия | Принято |
| 6-12 | [ru/6-12_denoising_ae.html](ru/6-12_denoising_ae.html) | Шумоподавляющий автоэнкодер | Группа сжатия | Принято |
| 6-13 | [ru/6-13_vae.html](ru/6-13_vae.html) | VAE | Группа генерации | Отложено |
| 6-14 | [ru/6-14_gan.html](ru/6-14_gan.html) | GAN | Группа генерации | Отложено |
| 6-15 | [ru/6-15_diffusion.html](ru/6-15_diffusion.html) | Диффузионная модель | Группа генерации | Отложено (окончательно) |

## В каждой главе

- Анкета, стр. 1 — сводка на одной странице
- Сцены собеседования, практикумы с обучением прямо в браузере, анимированные схемы, проверочные вопросы
- Пересдача (апелляция) — кандидат приводит доводы и сдаёт заново по заранее зарегистрированным условиям
- Код для Colab (PyTorch) — копирование, скачивание .py / .ipynb; на странице показан реальный результат запуска
- Поиск ошибок в коде ИИ-ассистента, промпты для ИИ, глоссарий, аналогии, источники
- Советы для преподавателей

## Данные

- Группа табличных данных (6-1 – 6-3): UCI Machine Learning Repository, Concrete Compressive Strength (Yeh, 1998, 1 030 составов, CC BY 4.0)
- Остальные главы (6-4 – 6-15): встроенные в scikit-learn рукописные цифры load_digits (1 797 изображений)

Каждый HTML-файл содержит изображения, данные и скрипты внутри — достаточно открыть его в браузере (только шрифты загружаются из Google Fonts). Ссылки между главами работают при той же структуре папок, поэтому не переименовывайте файлы. Первый открытый набор (машинное обучение) — в отдельном репозитории.

---

# Hội đồng Tuyển dụng Mô hình, Đợt tuyển dụng thứ hai — phỏng vấn mười lăm ứng viên học sâu

Nhà máy bê tông mở đợt tuyển dụng thứ hai. Ứng viên là mười lăm mạng nơ-ron, từ perceptron đến mô hình khuếch tán; muốn trúng tuyển, mỗi ứng viên phải vượt tiền bối đã trúng tuyển ở đợt thứ nhất (KNN, SVM, GBM, GMM, PCA…) trong cùng điều kiện. Phán quyết dựa trên trung bình của năm seed được huấn luyện thật trên Colab (PyTorch); ứng viên bị tạm hoãn có thể kháng nghị một lần để thi lại theo điều kiện đã đăng ký trước. Kết quả: 3 người trúng tuyển (1 người khi thi lại), 12 người tạm hoãn — "học sâu không phải lúc nào cũng thắng".

- Tác giả: Ahn Sangsun (Giám đốc M-Robo Co., Ltd.)
- Giấy phép: CC BY-NC 4.0 (sử dụng phi thương mại, bắt buộc ghi nguồn) — [LICENSE.md](LICENSE.md)
- Bắt đầu: [vi/index.html](vi/index.html)

## Danh sách các tập

Hãy xem bản đồ tổng thể ở 6-0 (thông báo tuyển dụng đợt hai và bảng tóm tắt học sâu) trước; mỗi tập kết thúc đều quay về 6-0.

| Tập | Tệp | Tiêu đề | Nhóm | Phán quyết |
|---|---|---|---|---|
| 6-0 | [vi/6-0_job_posting.html](vi/6-0_job_posting.html) | Thông báo tuyển dụng đợt hai · Bảng tóm tắt học sâu | Thông báo tuyển dụng |  |
| 6-1 | [vi/6-1_perceptron.html](vi/6-1_perceptron.html) | Perceptron | Nhóm Dữ liệu bảng | Trúng tuyển khi thi lại |
| 6-2 | [vi/6-2_mlp.html](vi/6-2_mlp.html) | Perceptron nhiều tầng | Nhóm Dữ liệu bảng | Tạm hoãn (chung cuộc) |
| 6-3 | [vi/6-3_resnet.html](vi/6-3_resnet.html) | ResNet | Nhóm Dữ liệu bảng | Tạm hoãn |
| 6-4 | [vi/6-4_cnn.html](vi/6-4_cnn.html) | CNN | Nhóm Hình ảnh | Tạm hoãn (chung cuộc) |
| 6-5 | [vi/6-5_siamese.html](vi/6-5_siamese.html) | Mạng Siamese | Nhóm Hình ảnh | Tạm hoãn (chung cuộc) |
| 6-6 | [vi/6-6_rnn.html](vi/6-6_rnn.html) | RNN | Nhóm Chuỗi | Tạm hoãn |
| 6-7 | [vi/6-7_lstm.html](vi/6-7_lstm.html) | LSTM | Nhóm Chuỗi | Tạm hoãn (chung cuộc) |
| 6-8 | [vi/6-8_gru.html](vi/6-8_gru.html) | GRU | Nhóm Chuỗi | Tạm hoãn (chung cuộc) |
| 6-9 | [vi/6-9_transformer.html](vi/6-9_transformer.html) | Transformer | Nhóm Chú ý | Tạm hoãn (chung cuộc) |
| 6-10 | [vi/6-10_som.html](vi/6-10_som.html) | SOM | Nhóm Phân cụm | Tạm hoãn |
| 6-11 | [vi/6-11_autoencoder.html](vi/6-11_autoencoder.html) | Autoencoder | Nhóm Nén | Trúng tuyển |
| 6-12 | [vi/6-12_denoising_ae.html](vi/6-12_denoising_ae.html) | Autoencoder khử nhiễu | Nhóm Nén | Trúng tuyển |
| 6-13 | [vi/6-13_vae.html](vi/6-13_vae.html) | VAE | Nhóm Sinh dữ liệu | Tạm hoãn |
| 6-14 | [vi/6-14_gan.html](vi/6-14_gan.html) | GAN | Nhóm Sinh dữ liệu | Tạm hoãn |
| 6-15 | [vi/6-15_diffusion.html](vi/6-15_diffusion.html) | Mô hình khuếch tán | Nhóm Sinh dữ liệu | Tạm hoãn (chung cuộc) |

## Mỗi tập gồm

- Hồ sơ ứng tuyển, trang 1 — tóm tắt một trang
- Cảnh phỏng vấn, bài thực hành tự huấn luyện trên trình duyệt, hình động, câu hỏi kiểm tra
- Thi lại (kháng nghị) — ứng viên đưa ra lý do và thi lại theo điều kiện đã đăng ký trước
- Mã Colab (PyTorch) — sao chép, tải .py / .ipynb; trang có kết quả chạy thật
- Tìm lỗi trong mã của trợ lý AI, prompt ứng dụng AI, bảng thuật ngữ, phép ẩn dụ, tài liệu tham khảo
- Gợi ý cho giáo viên

## Dữ liệu

- Nhóm Dữ liệu bảng (6-1 – 6-3): UCI Machine Learning Repository, Concrete Compressive Strength (Yeh, 1998, 1,030 cấp phối, CC BY 4.0)
- Các tập khác (6-4 – 6-15): chữ số viết tay load_digits có sẵn trong scikit-learn (1,797 ảnh)

Mỗi tệp HTML chứa sẵn hình ảnh, dữ liệu và script, chỉ cần mở bằng trình duyệt (chỉ phông chữ tải từ Google Fonts). Liên kết giữa các tập hoạt động với cùng cấu trúc thư mục, vì vậy đừng đổi tên tệp. Đợt tuyển dụng thứ nhất (học máy) nằm ở kho lưu trữ riêng.

---
