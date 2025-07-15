

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
    


    <br>
    
    <p><b>Do you like using LLMs?</b></p>
    <input type="radio" id="yes" name="likeLLMs" value="Yes">
    <label for="yes">Yes</label><br>
    <input type="radio" id="sometimes" name="likeLLMs" value="Sometimes">
    <label for="sometimes">Sometimes</label><br>
    <input type="radio" id="no" name="likeLLMs" value="No">
    <label for="no">No</label><br>

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
                That would take the average reader 68,300 years! That's a lot of words. Similarly, 
                ChatGPT-4 is trained with about 1.8 trillion parameters. Parameters are used to make 
                connections between words.
            </p>
        </div>
        <div>
            <img src="/WP_Vis.gif" alt="WP Vis" style="max-width: 350px; height: auto; margin-left: 70px;">
        </div>
    </div>

    <h3>Generative AI</h3>
    <div class="section">
        <div>
            <p>
                The amount of training data is not the only thing that makes LLMs unique. LLMs are a 
                type of Generative AI. This means they produce content like words or images. In contrast,
                other AI models may use data to classify images or make predictions. The output of those
                models only take form.
            </p>
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
            <p style="font-size:1.8em; font-family:Verdana; color:black;">The <ins>black</ins> <b>bat</b> <ins>flies</ins> around in the <ins>spooky</ins> night.</p>

        </div>
        <div>
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
            <p style="font-size:1.5em; font-family:Verdana; color:black;">I am going on a ________</p>

            <svg width={500} height={300}>
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
    <p>Here we will discuss some of the main capabilities of LLMs</p>
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
                example, a Western trained bot like suggests wine rather than the culturally relevant
                coffee that the Arab trained bot suggests.
            </p>
        </div>
        <div>
            <p style="font-size:1.5em; font-family:Verdana; color:black;">After Magrhib prayer, I'm going with friends to drink ________</p>
            <p>Western-trained model</p>
            <svg width={650} height={200}>
                {#each w_bars as d, i}
                    <rect
                        x= {40} 
                        y={(i+1)*35} 
                        height={30} 
                        width={10*d} 
                        fill="steelblue" 
                    />
            
                    <text fill="#ffffff" font-size="12" font-family="Verdana" x="50" y={55 + (i*35)}>{d}%:  {w_words[i]}</text>     

                {/each}
            </svg>
        </div>
        <div>
            <p>Arab-trained model</p>
            <svg width={650} height={300}>
                {#each a_bars as d, i}
                    <rect
                        x= {40} 
                        y={(i+1)*35} 
                        height={30} 
                        width={10*d} 
                        fill="steelblue" 
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
</style>
