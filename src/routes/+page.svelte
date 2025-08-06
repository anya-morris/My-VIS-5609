

<h1 style="text-align:center">What can LLMs really do?</h1>
<p style="text-align: center">By: Anya Morris</p>
<br>

<div class="section">
    <h2>Feelings on LLMs</h2> 
    <div>
        <p>
            LLMs are increasingly becoming a part of everday life. A recent study observed
            that 52% of American adults use LLMs like ChatGPT and Claude. Some people
            use them to answer questions, organize daily tasks, or even as  a form of
            interaction. However, many people don't know how they work. Let's take a 
            look at the inner workings of LLMs to determine what they are capable of and 
            how they are limited.
        </p>
    
    </div>
    <div>
        <img src="./UsageChart2.png" alt="Usage Chart" style="max-width: 550px; height: auto; margin-left: 70px;">
    </div>
    <br>
    <div>
    <p><b>Do you like using LLMs?</b></p>
    <input type="radio" id="yes" name="likeLLMs" value="Yes">
    <label for="yes">Yes</label><br>
    <input type="radio" id="sometimes" name="likeLLMs" value="Sometimes">
    <label for="sometimes">Sometimes</label><br>
    <input type="radio" id="no" name="likeLLMs" value="No">
    <label for="no">No</label><br>

    <p><b>How often do you use LLMs?</b></p>
    <input type="radio" id="never" name="useLLMs" value="Never">
    <label for="never">Never</label><br>
    <input type="radio" id="Month" name="useLLMs" value="Month">
    <label for="Month">Once a month</label><br>
    <input type="radio" id="week" name="useLLMs" value="Once a week">
    <label for="week">Once a week</label><br>
    <input type="radio" id="multWeek" name="useLLMs" value="Multiple a week">
    <label for="multWeek">Multiple times a week</label><br>
    <input type="radio" id="day" name="useLLMs" value="Every day">
    <label for="day">Every day</label><br>

    <p><b>What do you like about LLMs?</b></p>
    <input type="checkbox" id="fun" name="positives" value="Fun to use">
    <label for="fun">They are fun and friendly to talk to</label><br>
    <input type="checkbox" id="helpful" name="positives" value="Help with tasks">
    <label for="helpful">They help me with day to day tasks</label><br>
    <input type="checkbox" id="clarity" name="positives" value="Clarity">
    <label for="clarity">They give clear, synthesized responses</label><br>
    <input type="checkbox" id="lengthy" name="positives" value="lengthy">
    <label for="lengthy">They give long responses</label><br>
    <input type="checkbox" id="better" name="positives" value="Work better">
    <label for="better">They work better than other technology at certain tasks</label><br>
    <input type="checkbox" id="nothing" name="positives" value="Nothing">
    <label for="nothing">Nothing</label><br>

    <p><b>What do you dislike about LLMs?</b></p>
    <input type="checkbox" id="biased" name="negatives" value="Biased">
    <label for="biased">They are biased</label><br>
    <input type="checkbox" id="intent" name="negatives" value="Misunderstand">
    <label for="misunderstand">They never understand my prompt or intent</label><br>
    <input type="checkbox" id="transparency" name="negatives" value="Transparency">
    <label for="transparency">I don't understand how they work</label><br>
    <input type="checkbox" id="inaccurate" name="negatives" value="Inaccurate">
    <label for="inaccurate">They give inaccurate information</label><br>
    <input type="checkbox" id="scared" name="negatives" value="Scared">
    <label for="scared">I'm worried they will take over basic tasks</label><br>
    <input type="checkbox" id="refuse" name="negatives" value="Refuse">
    <label for="refuse">They refuse to answer certain prompts</label><br>
    <input type="checkbox" id="nothing" name="negatives" value="Nothing">
    <label for="nothing">Nothing</label><br>
    </div>
</div>
<br>
<br>
<br>
<br>

<script>
    

    let bars = [29, 27, 20, 14, 10]
    let words = ["trip", "mission", "vacation", "tour", "date"]
    let word = "trip"
    let w_bars = [50, 30, 20]
    let w_words = ["wine", "whisky", "hibiscus"]
    let a_bars = [55, 35, 10]
    let a_words = ["coffee", "tequila", "mocha"]
    let s_words = ["stage", "game", "dream", "lie"]
    let s_bars = [74, 11, 9, 6]

    var i = 0;
    var txt = 'I am going on a...';
    var speed = 50;

    function typeWriter() {
        if (i < txt.length) {
            document.getElementById("demo").innerHTML += txt.charAt(i);
            i++;
            setTimeout(typeWriter, speed);
        }
        
    }
</script>

<div>
    <h2>How do LLMs work?</h2>
    <h3>Training Data</h3>
    <div class='section'>
        <div>
            
            <p>
                LLMs are trained on a massive amount of data. Meta's Llama, for example, is trained on
                15 trillion tokens which is equivalent to about 11 trillion English words. Processing
                11 trillion words is about the same as reading <i>War and Peace</i> 19 million times. 
                <i>War and Peace</i> is 2 inches thick, so stacking it on top of itself 19 million 
                could make it to the International Space Station 2.4 times. That's a lot of words! Similarly, 
                ChatGPT-4 is trained with about 1.8 trillion parameters. Parameters are used to make 
                connections between words.
            </p>
        </div>
        <div>
            <img src="./WP_Vis.gif" alt="WP Vis" style="max-width: 350px; height: auto; margin-left: 20px;">
            <img src="./WP_Visual2.png" alt="WP Vis2" style="max-width: 200px; height: auto; margin-left: 30px;">
        </div>
    </div>

    <h3>Generative AI</h3>
    <div class="section">
        <div>
            <p>
                The amount of training data is not the only thing that makes LLMs unique. LLMs are a 
                type of Generative AI. This means they produce content like words or images. In contrast,
                other AI models may use data to classify images or make predictions. Instead of text of images, 
                the output of non-generative AI models might be a classification or number. For example, a 
                classification model may be trained to distinguish images or dogs from images of cats.
            </p>
        </div>

        <div>
            <img src="./GenAI.png" alt="WP Vis" style="max-width: 280px; height: auto; margin-left: 20px;">
            <img src="./ClassAI.png" alt="WP Vis2" style="max-width: 280px; height: auto; margin-left: 20px;">
        </div>
    </div>


    <h3>Pretraining</h3>
    <div class="section">
        <div>
            <p>
                Once all of the data is gathered to train an LLM is separated into tokens. Each token is 
                passed through a series of layers to determine its meaning based on the context of other
                words around it. For example, it may consider the words "black", "flies", and "spooky" to 
                determine that this sentence is talking about an animal bat, not a baseball bat. At the 
                end of this process, the model has a good sense of how the language works. It even memorizes 
                some chunks of data, sometimes whole paragraphs, that it may 
                spit out later when it is generating text.
            </p>
        </div>
        <div>
            <p class="speech-bubble">
                <img src="./Human.png" alt="Human icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
                The <ins>black</ins> <b>bat</b> <ins>flies</ins> around in the <ins>spooky</ins> night.
            </p>

        </div>
        <div class="response">
            <img src="./Bat1.png" alt="Bat animal" style="max-width: 250px; height: auto; padding: 10px; margin-left: 25px;">
            <img src="./Bat2.png" alt="Baseball bat" style="max-width: 250px; height: auto; padding: 10px;">

        </div>
        
        
    </div>
    

    <h3>Word Predictions</h3>
    <div class="section">
        <div>
            <p>
                Once an LLM has been trained to understand language, it can take input and determine the 
                next most likely word using statistics. It again uses the context of the words around it
                in order to decide which word is the next best fit.
            </p>
        </div>
        <div>   
                    
            <p class="speech-bubble" id="demo" style="height:30px">
                <img src="./Human.png" alt="Human icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
               I am going on a...
            </p>
        </div>
        <div class="response">
            <img src="./RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
            <svg width={500} height={250}>
                {#each bars as d, i}
                    <rect
                    x= {40} 
                    y={(i+1)*35} 
                    height={30} 
                    width={10*d} 
                    fill="steelblue" 
                    />
            
                    <text fill="#ffffff" font-size="12" font-family="Verdana" x="50" y={55 + (i*35)}>{d}%:  {words[i]}</text>     

            
                {/each}
            </svg>
        </div>
    </div>
    
    <br>
    
</div>
<br>
<br>
<br>
<br>
<div>
    <h2>Capabilities</h2>
    
    <div class="section">
        <h3>Style Imitation</h3>
        <div>
            <p>
                One of LLMs' most effective capabilities is style imitation. If an LLM has enough
                data on the language of a certain person, time period, or genre, it can imitate the 
                style of that thing. For example, ChatGPT has a lot of data on Shakespeare because
                he is so prominent in English culture. Therefore, it is really good at recognizing
                Shakespeare's work and imitating it. It can easily fill in his famous quotes, as 
                shown in this output.
            </p>
        </div>
        <div>
            <p class="speech-bubble">
                <img src="./Shakespeare.png" alt="Shakespeare icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
                All the world's a...
            </p>
        </div>
        <div class="response">
            <img src="./RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
            <svg width={500} height={200}>
                {#each s_bars as d, i}
                    <rect
                    x= {0} 
                    y={(i+1)*35} 
                    height={30} 
                    width={10*d} 
                    fill="steelblue" 
                    />
            
                    <text fill="#ffffff" font-size="12" font-family="Verdana" x="5" y={55 + (i*35)}>{d}%:  {s_words[i]}</text>     

            
                {/each}
            </svg>
        
        </div>
    </div>
</div>
<br>
<br>
<br>
<br>
<div>

    
    <h2>Limitations</h2>
    <h3>Bias</h3>
    <div class="section">
        <div>
            <p>As powerful as LLMs can be, they have some limitations. First, the training data is 
                inevitably biased. LLMs are trained largely on data from the Western world, so they 
                are less likely to give accurate information on non-Western cultures and ideas. 
                Think back to the word prediction process: if an LLM is trained on Western data then
                it is much more likely to predict words that are relevant to Western culture. For 
                example, a Western trained bot suggests wine or whiskey rather than the culturally relevant
                coffee that the Arab trained bot suggests. Someone in a Western culture might not know to 
                question this inaccurate information.
            </p>
        </div>
        <div>
            <p class="speech-bubble">
                <img src="./ArabAvatar.png" alt="Arab Human icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
                After Maghrib prayer, I'm going with friends to drink...
            </p>
        </div>
        <div class="response">
            <p>Western-trained model</p>
            <img src="./RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
            <svg width={650} height={150}>
                {#each w_bars as d, i}
                    <rect
                        x= {40} 
                        y={(i+1)*35} 
                        height={30} 
                        width={10*d} 
                        fill="firebrick" 
                    />
            
                    <text fill="#ffffff" font-size="12" font-family="Verdana" x="50" y={55 + (i*35)}>{d}%:  {w_words[i]}</text>     

                {/each}
            </svg>
        
        </div>
        <br>
        <div class="response" style="margin-top: 20px;">
            <p>Arab-trained model</p>
            <img src="./RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
            <svg width={650} height={150}>
                {#each a_bars as d, i}
                    <rect
                        x= {40} 
                        y={(i+1)*35} 
                        height={30} 
                        width={10*d} 
                        fill="forestgreen" 
                    />
                    
                    <text fill="#ffffff" font-size="12" font-family="Verdana" x="50" y={55 + (i*35)}>{d}%:  {a_words[i]}</text>     
        
                    
               {/each}
            </svg>
        </div>
    </div>
    

</div>
<div>
    <h2>Conclusion</h2>

    <div class="section">
        <div>
            <p>LLMs can be great tools using their vast data and statistical prediction
            power. However, it is important to understand at least basically how they
            work before determining what they should be used for. They are good at 
            tasks like imitation, summarization, and easy explanations, but problems
            arrive when those tasks are attempted when there are holes in the data set.
            Always remember what bias might be worked into a model and how that affects
            the task you are asking it to complete.
            </p>
        </div>

    </div>
</div>
<div>
    <h3>Sources</h3>

    <p>
        3Blue1Brown. (2024, April 1). But what is a GPT? Visual intro to Transformers | Deep learning, chapter 5. Www.youtube.com. https://www.youtube.com/watch?v=wjZofJX0v4M
        <br>
        Almeida, D., Shmarko, K., & Lomas, E. (2022). The ethics of facial recognition technologies, surveillance, and accountability in an age of artificial intelligence: a comparative analysis of US, EU, and UK regulatory frameworks. AI and Ethics, 2(3), 377–387. https://doi.org/10.1007/s43681-021-00077-w
        <br>
        Backlinko team. (2024, June 4). ChatGPT Statistics 2024: How Many People Use ChatGPT? Backlinko. https://backlinko.com/chatgpt-stats
        <br>
        Briganti, G. (2023). How ChatGPT works: a mini review. European Archives of Oto-Rhino-Laryngology, 281(3). https://doi.org/10.1007/s00405-023-08337-7
        <br>
        Buolamwini, J. (2023, November 8). “If you have a face, you have a place in the conversation about AI”, experts say (T. Mosley, Interviewer) [Interview]. In NPR.
        <br>
        Cho, A., Kim, G., Karpekov, A., Helbling, A., Wang, J., Lee, S., Hoover, B., & Chau, P. (2017). Transformer Explainer: LLM Transformer Model Visually Explained. Github.io. https://poloclub.github.io/transformer-explainer/
        <br>
        Coursera. (2023, January 12). 4 Types of AI: Getting to Know Artificial Intelligence. Coursera. https://www.coursera.org/articles/types-of-ai
        <br>
        Dorr, L. (2022). Types of Artificial Intelligence, Explained. Www.dentalproductsreport.com, 56. https://www.dentalproductsreport.com/view/types-of-artificial-intelligence-explained
        <br>
        Gherheş, V. (2018). Why Are We Afraid of Artificial Intelligence (Ai)? European Review of Applied Sociology, 11(17), 6–15. https://doi.org/10.1515/eras-2018-0006
        <br>
        Hartmann, V., Suri, A., Bindschaedler, V., Evans, D., Tople, S., & West, R. (2023). SoK: Memorization in General-Purpose Large Language Models. https://arxiv.org/pdf/2310.18362
        <br>
        Hayati, S., Lee, M., Rajagopal, D., & Kang, D. (2024). How Far Can We Extract Diverse Perspectives from Large Language Models? arXiv.
        <br>
        Howarth, J. (2024, August 6). Number of Parameters in GPT-4 (Latest Data). Exploding Topics; Exploding Topics. https://explodingtopics.com/blog/gpt-parameters
        <br>
        IBM Data and AI Team. (2023, October 12). Types of Artificial Intelligence | IBM. Www.ibm.com; IBM. https://www.ibm.com/think/topics/artificial-intelligence-types
        <br>
        Kim, Y., Lee, J., Kim, S., Park, J., & Kim, J. (2024). Understanding Users’ Dissatisfaction with ChatGPT Responses: Types, Resolving Tactics, and the Effect of Knowledge Level. ACM. https://doi.org/10.1145/3640543.3645148
        <br>
        Lee, S., Hoover, B., Strobelt, H., Wang, Z. J., Peng, S., Wright, A., Li, K., Park, H., Yang, H., & Chau, D. H. (2023, May 8). Diffusion Explainer: Visual Explanation for Text-to-image Stable Diffusion. ArXiv.org. https://doi.org/10.48550/arXiv.2305.03509
        <br>
        Li, J., Zhou, F., Sun, S., Zhang, Y., Zhao, H., & Liu, P. (2024). Dissecting Human and LLM Preferences. ArXiv, abs/2402.11296.
        <br>
        meta-llama. (2024). llama-models/models/llama3_1/MODEL_CARD.md at main · meta-llama/llama-models. GitHub. https://github.com/meta-llama/llama-models/blob/main/models/llama3_1/MODEL_CARD.md
        <br>
        Naik, D., Naik, I., & Naik, N. (2024). Large Data Begets Large Data: Studying Large Language Models (LLMs) and Its History, Types, Working, Benefits and Limitations. Lecture Notes in Networks and Systems, 293–314. https://doi.org/10.1007/978-3-031-74443-3_18
        <br>
        Naous, T., Ryan, M., Ritter, A., & Xu, W. (2024). Having Beer after Prayer? Measuring Cultural Bias in Large Language Models. https://arxiv.org/pdf/2305.14456
        <br>
        Pellegrino, M., & Kelly, R. (2019). Intelligent machines and the growing importance of ethics. JSTOR. https://www.jstor.org/stable/resrep19966.11
        <br>
        Prompt Engineering. (2025, June 7). Www.promptingguide.ai; DAIR.AI. https://www.promptingguide.ai/techniques/cot
        <br>
        Riemer, K., & Peter, S. (2024). Conceptualizing generative AI as style engines: Application archetypes and implications. International Journal of Information Management, 79, 102824–102824. https://doi.org/10.1016/j.ijinfomgt.2024.102824
        <br>
        Schepman, A., & Rodway, P. (2020). Initial validation of the general attitudes towards Artificial Intelligence Scale. Computers in Human Behavior Reports, 1. https://doi.org/10.1016/j.chbr.2020.100014
        <br>
        Shankar, S., Halpern, Y., Breck, E., Atwood, J., Wilson, J., & Sculley, D. (2017). No Classification without Representation: Assessing Geodiversity Issues in Open Data Sets for the Developing World. arXiv.
        <br>
        Townsend, E. (2025, March 12). Survey: 52% of U.S. adults now use AI large language models like ChatGPT. Today at Elon. https://www.elon.edu/u/news/2025/03/12/survey-52-of-u-s-adults-now-use-ai-large-language-models-like-chatgpt/
        <br>
        Wei, J. Z., Wang, X., Schuurmans, D., Bosma, M., Chi, E. H., Le, Q. V., & Zhou, D. (2022). Chain-of-Thought Prompting Elicits Reasoning in Large Language Models. arXiv. https://doi.org/10.48550/arxiv.2201.11903
        <br>
        Yang, J., Jin, H., Tang, R., Han, X., Feng, Q., Jiang, H., Zhong, S., Yin, B., & Hu, X. (2024). Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond. ACM Transactions on Knowledge Discovery from Data. https://doi.org/10.1145/3649506

    </p>

</div>


<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Archivo:ital,wght@0,100..900;1,100..900&family=Red+Hat+Display:ital,wght@0,300..900;1,300..900&display=swap" rel="stylesheet">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,200..1000;1,200..1000&display=swap" rel="stylesheet">

<style> 
    :global(body) {
        background-color: mintcream;
        margin-left: 50px;
        
    }
    h1 {
        font-family: "Archivo", sans-serif;
        color: midnightblue;
        font-size: 4em;
        max-width: 5000px;
        text-align: center;
        }
    h2 {
        font-family: "Nunito", sans-serif;
        color: midnightblue;
        font-size: 2.7em;
        
    }
    h3 {
        font-family: "Nunito", sans-serif;
        color: midnightblue;
        font-size: 2em;
    }
    p {
        font-family: "Nunito", sans-serif;
        color: midnightblue;
        font-size: 1.5em;
        
    }
    label {
        font-family: "Nunito", sans-serif;
        font-size: 1.5em;
        
    }

    div.section {
        width: 100%;
        overflow: auto;
    }
    div.section div {
        width: 45%;
        float: left;
        margin-right: 20px;
    }
    div.section div.response{
        position: relative;
	    background-color: rgb(227, 227, 227);
        width: 600px;
	    border-radius: 10px;
        border-style: solid;
        border-width: 10px;
        border-color: rgb(227, 227, 227);
        font-family:Verdana;
    }
    p.speech-bubble {
	    position: relative;
	    background-color: #a5e3e9;
        width: 600px;
	    border-radius: 10px;
        border-style: solid;
        border-width: 10px;
        border-color: #a5e3e9;
        font-family:Verdana;
        color: black;
    }
    
</style>
