# Editorial Summarization

<img src="https://github.com/user-attachments/assets/dd9afa3d-4b06-4a8b-9d07-997b4043cea6" width="400"/>
<img src="https://github.com/user-attachments/assets/6e50af4f-8a92-40f2-9ccf-917cd237e4a1" width="200"/>
<img src="https://github.com/user-attachments/assets/173cf1ea-07af-4c74-a26a-6e560a7217a9" width="400" height="250"/>
Now a days , the amount of information is available is growing rapidly. However, readers often find it hard to go through long articles and stay up 
to date with important news. The goal is to create a model that can automatically summarize Editorials from The Hindu Newspaper by keeping the important details and the main message. The summary should focus on the most important information and present it in a short and clear way. This will allow readers to quickly understand the main points of the news without having to read the entire article.

# Model Architecture
We use the T5 model, which is a Transformer based text-to-text model that converts an article into a summary.


T5 stands for Text-To-Text Transfer Transformer.
Based on encoder-decoder architecture:
* Encoder: Reads and understands the input text (e.g., news article).
* Decoder: Generates the target text (e.g., summary).

Pre-trained on large datasets → fine-tuned on our domain-specific editorial data.
During fine-tuning, it learns from pairs of articles and their summaries.
The model generates a short, clear summary using its learned patterns.

# Innovation
Focus on Editorials:  We specifically targeted editorial articles,this is especially helpful for government exam aspirants, who regularly read editorials for current affairs and critical analysis.

Fine-Tuned for Better Performance:  By training the T5 model on our custom editorial dataset, we achieved better results than using general pretrained models.

For Example:  Generic tools like ChatGPT are limited in handling multiple or large images at once. But our system can process many editorial images efficiently.
# Conclusion
  In this project, we worked on summarizing editorials from The Hindu newspaper using a fine-tuned T5 model.  Unlike general pretrained models, our approach involved creating a manual, domain-specific dataset, resulting  in more accurate summaries.We used OCR to get text from images and cleaned the text before giving it to the model. This made our summaries more accurate and useful, especially for students and people preparing for government exams.

 As we include more editorial articles in the dataset, the model learns better and produces more accurate summaries. Overall, our method gives better results than using already trained models that are not focused on editorials.
