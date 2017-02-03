# Memory

<h1>Groovy check time</h1>
<pre>
@Field startTime

def startTimer() {
    startTime = System.nanoTime();
}

def endTimer(def message) {
    long endTime = System.nanoTime();
    long duration = (endTime - startTime);
    def result = duration / 1000000
    logger.error("Hello " + message + " " + result)
}
</pre>
