<div class="quick-pairing">
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">1+0</div>
    <div class="quick-pairing__perf">Bullet</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">2+1</div>
    <div class="quick-pairing__perf">Bullet</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">3+0</div>
    <div class="quick-pairing__perf">Blitz</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">3+2</div>
    <div class="quick-pairing__perf">Blitz</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">5+0</div>
    <div class="quick-pairing__perf">Blitz</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">5+3</div>
    <div class="quick-pairing__perf">Blitz</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">10+0</div>
    <div class="quick-pairing__perf">Rapid</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">10+5</div>
    <div class="quick-pairing__perf">Rapid</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">15+10</div>
    <div class="quick-pairing__perf">Rapid</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">30+0</div>
    <div class="quick-pairing__perf">Classical</div>
  </div>
  <div class="quick-pairing__item">
    <div class="quick-pairing__clock">30+20</div>
    <div class="quick-pairing__perf">Classical</div>
  </div>
  <div class="quick-pairing__item quick-pairing__item--custom">
    <div class="quick-pairing__clock">Custom</div>
    <div class="quick-pairing__perf">&nbsp;</div>
  </div>
</div>

<style>
.quick-pairing {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 1rem;
  padding: 1rem;
  background-color: #f1f1f1;
}

.quick-pairing__item {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 120px;
  height: 120px;
  background-color: #fff;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease-in-out;
}

.quick-pairing__item:hover {
  background-color: #dcdcdc;
}

.quick-pairing__clock {
  font-size: 30px;
  font-weight: bold;
  margin-bottom: 10px;
  text-align: center;
}

.quick-pairing__perf {
  font-size: 18px;
  color: #666;
  text-align: center;
}

.quick-pairing__item--custom {
  background-color: #ccc;
}

@media screen and (max-width: 768px) {
  .quick-pairing {
    padding: 0.5rem;
  }
  
  .quick-pairing__item {
    width: 100px;
    height: 100px;
    font-size: 0.8rem;
  }
  
  .quick-pairing__clock {
    font-size: 1.2rem;
    margin-bottom: 0.5rem;
  }
  
  .quick-pairing__perf {
    font-size: 0.8rem;
  }
}

@media screen and (min-width: 769px) and (max-width: 1023px) {
  .quick-pairing {
    max-width: 600px;
    margin: 0 auto;
  }
  
  .quick-pairing__item {
    width: 150px;
    height: 150px;
    font-size: 1rem;
  }
}

@media screen and (min-width: 1024px) {
  .quick-pairing {
    max-width: 800px;
    margin: 0 auto;
    flex-wrap: nowrap;
  }
  
  .quick-pairing__item {
    width: 180px;
    height: 180px;
    font-size: 1.2rem;
  }
  
  /* Adjust margin for each item */
  .quick-pairing__item:not(:last-child) {
    margin-bottom: 1rem;
  }
  
  /* Three columns for desktop view */
  .quick-pairing__item:nth-child(3n+1) {
    margin-right: 1rem;
  }
  
  /* Three rows for desktop view */
  .quick-pairing__item:nth-child(9n+1) {
    margin-top: 0;
  }
  
  .quick-pairing__item:nth-child(n+10) {
    margin-top: 1rem;
  }
}

</style>
