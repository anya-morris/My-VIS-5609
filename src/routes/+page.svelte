

<h1 style="text-align:center">What can LLMs really do?</h1>
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
        <img src="/UsageChart.png" alt="Usage Chart" style="max-width: 350px; height: auto; margin-left: 70px;">
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
            <img src="/WP_Vis.gif" alt="WP Vis" style="max-width: 350px; height: auto; margin-left: 20px;">
            <img src="/WP_Visual2.png" alt="WP Vis2" style="max-width: 200px; height: auto; margin-left: 30px;">
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
            <img src="/GenAI.png" alt="WP Vis" style="max-width: 280px; height: auto; margin-left: 20px;">
            <img src="/ClassAI.png" alt="WP Vis2" style="max-width: 280px; height: auto; margin-left: 20px;">
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
                <img src="/Human.png" alt="Human icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
                The <ins>black</ins> <b>bat</b> <ins>flies</ins> around in the <ins>spooky</ins> night.
            </p>

        </div>
        <div class="response">
            <img src="/Bat1.png" alt="Bat animal" style="max-width: 250px; height: auto; padding: 10px; margin-left: 25px;">
            <img src="/Bat2.png" alt="Baseball bat" style="max-width: 250px; height: auto; padding: 10px;">

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
            <p class="speech-bubble">
                <img src="/Human.png" alt="Human icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
                I am going on a...</p>
        </div>
        <div class="response">
            <img src="/RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
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
        <h3>Summarization</h3>
        <div>
            <p>One of LLMs' most effective capabilities is text summarization. This makes
                sense given what we now know about word predictions. It's much easier to 
                predict the next most likely word when all the words are provided to the 
                LLM through the piece that you want summarized. LLMs use two different 
                summarization techniques. Either they extract sentences directly from the text 
                or they create an abstract summary with their own creativity. Usually these
                techniques are combined for the best results, but both use statistics to 
                predict words. 
            </p>
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
                <img src="/ArabAvatar.png" alt="Arab Human icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
                After Maghrib prayer, I'm going with friends to drink...
            </p>
        </div>
        <div class="response">
            <p>Western-trained model</p>
            <img src="/RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
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
            <img src="/RobotIcon.png" alt="Robot icon" style="border-radius: 3px; max-width: 30px; height: auto; float:left; margin-right: 10px;">
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
        margin-right: 60px;
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
