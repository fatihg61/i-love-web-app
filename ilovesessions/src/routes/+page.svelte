<script>
    import Header from "../lib/components/Header.svelte";
    import Footer from "../lib/components/Footer.svelte";
</script>

<svelte:head>
    <title>We love web app</title>
</svelte:head>

<Header />

<h1 class="header-title">The we love web sessions blog by me FG!</h1>

<main>
    <div class="timeline">
        <div class="timeline-item">
          <h4>We ♥ Web 1: Masterclass AI by Fatih</h4>
          <p>No date</p>
          <p>Masterclass about how to utilize the use of AI in Front end</p>
          <br>
          <a href="/aimasterclass" class="add-button">Read More</a>
        </div>
      
        <div class="timeline-item">
          <h4>We ♥ Web 2: Yolijn van der Kolk</h4>
          <p>VRIJDAG 24/11/23</p>
          <p>TBD</p>
          <br>
        </div>
      
        <div class="timeline-item">
          <h4>We ♥ Web 3: Julie Miocene</h4>
          <p>VRIJDAG 15/12/23</p>
          <p>About CSS</p>
          <br>
        </div>
      </div>
</main>

<Footer />

<style>
.header-title {
  text-align: center;
}

.timeline {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  animation: timeline-appear 1s ease-in-out forwards;
}

@keyframes timeline-appear {
  from {
    opacity: 0;
    transform: translateY(50px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.timeline-item {
  margin-bottom: 20px;
  padding: 10px;
  border: 1px solid #ccc;
  width: 50%;
  animation: timeline-item-appear 1s ease-in-out forwards 0.2s;
}

@keyframes timeline-item-appear {
  from {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.timeline-item h4 {
  margin-bottom: 5px;
}

.timeline-item p {
  font-size: 14px;
}

.add-button {
  position: absolute;
  right: 20px;
  top: 50%;
  transform: translateY(-50%);
  background-color: #050542;
  color: #66e5bf;
  padding: 10px 20px;
  border: #66e5bf 1px solid;
  cursor: pointer;
  z-index: 1;
}

@media (max-width: 768px) {
  .add-button {
    position: static;
    display: block;
    margin: 20px auto;
    width: 100%;
  }
}

</style>