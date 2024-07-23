<!-- script to make the button functional -->
<script>
    let count = 0;
    function increment() {
        count += 1;
    }
</script>

<!-- adding everything in a div to center it on the page -->
<!-- creating 2 containers so that we can center everything -->
<div class="outer-container">
    <div class="container">
        <!-- heading -->
        <h1>Welcome to a random button I made</h1>

        <!-- button -->
        <button on:click={increment}>
            Clicked {count}
            {count === 1 ? "time" : "times"}
        </button>
    </div>
</div>

<!-- styling and centering -->
<style>
    .outer-container {
        display: flex;
        justify-content: center;
        /* aligning items to the top */
        align-items: flex-start;
        height: 100vh;
    }
    .container {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        text-align: center;
        /* adding a border around everything like a box */
        border: 2px solid rgb(128, 6, 46);
        /* adding padding inside the box */
        padding: 20px;
        /* making sure it doesn’t affect the overall size */
        box-sizing: border-box;
        max-height: 500px;
        max-width: 700px;
        /* to centre everything */
        margin: auto;
        border-radius: 20px;
        /* moving the outercontainer down as I like */
        margin-top: 300px;
    }
    button {
        background-color: pink;
        color: rgb(78, 0, 26);
        border-color: brown;
        border-radius: 20px;
        padding: 10px;
        align-items: center;
    }
    h1 {
        color: rgb(78, 0, 26);
        font-family: Arial, sans-serif;
    }
</style>
