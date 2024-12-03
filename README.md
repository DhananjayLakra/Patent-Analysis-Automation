# Patent-Analysis-Automation
A simple python script to automate the technological classification of patents.

Problem with Existing Classifications

Current CPC/IPC classifications of patents are often vague and provide limited insight into the technical domain of the patent. For example, the classification code for patent US9043608B2-G06F21/81 stands for "Protecting specific internal or peripheral components, in which the protection of a component leads to protection of the entire computer by operating on the power supply, e.g., enabling or disabling power-on, sleep, or resume operations." However, the patent itself discusses a method for cryptographic computation, which is its actual technical domain. This distinction is not evident from the existing classification, making it unreliable for precise technical categorization. This issue is further exacerbated when dealing with a large portfolio of patents, where manual classification becomes infeasible.

About the Program

This program automates technological analysis for batches of patents. Users can input the batch through an Excel file. The program scrapes the text from Google Patents pages using BeautifulSoup 4 and employs the NLTK module to extract relevant keywords, including bigrams and trigrams, from the patent text. These keywords, along with other markers such as the abstract and title, help provide a more accurate categorization of the patent's technical domain. 

Note: This program was developed by me during my current job and is shared here with the company's permission. The dataset contains a selection of random patents chosen by me.
