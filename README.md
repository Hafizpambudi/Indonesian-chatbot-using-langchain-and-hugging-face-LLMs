# Indonesian-chatbot-using-langchain-and-hugging-face-LLMs

# Chatbot Fresh Water Fish Knowledge 

## Teams 
- Hafiz Pambudi - ML engineer 
- Naufal Kanz - Design Researcher 
- Muhammad Daffa Ramadhan - Data Engineer
- Yerico Marchel Bernadus - ML Ops 

## Idea Background 

### 1. Theme 
tema : Aquakultur

### 2. Problem 

Masalah : Seringkali para pembudidaya dan para newbie dalam budidaya ikan air tawar merasa kebingungan ketika butuh informasi yang cepat dan akurat dalam 1 platform. 

### 3. Solution
Solusi : Membuat chatbot tentang Knowledge budidaya ikan air tawar yang berfokus pada 5 ikan berikut : 
- ikan lele 
- ikan bawal 
- ikan gurame 
- ikan mujair 
- ikan nila 
chatbot ini akan membantu user dalam mendapatkan informasi yang cepat dan akurat. 

## Dataset 
Chatbot akan menggunakan 5 document sebagai knowledge base. Dataset didapatkan dari pengumpulan dari berbagai situs terkait dengan budidaya ikan ikan berikut :  ikan lele, ikan bawal, ikan gurame, ikan nila dan ikan mujair. 
detail dataset : 

## Algorithm
Chatbot ini menggunakan algoritma RAG (Retrieval-Augmented Generation)  yang dipadukan dengan LLM dari hugging face. LLM yang digunakan merupakan llm yang khusus unutk melakukan percakapan bahasa indoensia. Algoritma ini dipilih dengan tujuan untuk mendapatkan percakapan dalam chatbot yang natural.  
LLM : kalisai/Nusantara-4b-Indo-Chat | sentence embedding : firqaaa/indo-sentence-bert-base


## Prototype
![chatbot](https://github.com/Hafizpambudi/Indonesian-chatbot-using-langchain-and-hugging-face-LLMs/assets/154437965/8906a0b4-e0e7-4911-b3c3-584887ce45c2)


## Integration 
Model ini akan diintegrasikan ke dalam platform mobile. Sehingga untuk mempermudah integrasi, Model yang telah dikembangan  disimpan dan dibuatkan menjadi API. API akan dibuangkus menjadi container menggunakan docker dan deploy secara public menggunakan service dari ibm code engine. 

## Deployment 
Setelah proses developing dan training model selesai dilakukan, chatbot akan dibuatkan menjadi API. Tujuan dibuatkannya api agar pihak developer mobile dimana fitur ini akan diimplementasikan, akan merasa dimudahkan. Pembuatan API menggunakan framework FAST Api. Ketika API selesai di develop, dilakukan kontainerisasi menggunakan docker dan dilakukan deployment ke dalam servide IBM code engine. Deployment ini akan menghasilkan public endpoint url yang siap di konsumsi oleh pihak developer mobile. 

## Result 
![image](https://github.com/Hafizpambudi/Indonesian-chatbot-using-langchain-and-hugging-face-LLMs/assets/154437965/6534522f-5fc6-447a-bc0c-a2260d5e8f15)
chatbot bisa menggenerate response dengan natural dengan waktu 12.67 sec 

## Conclusion 
chatbot model yang dibangun berhasil  memberikan response atas pertanyaan user dengan cukup natural. 
