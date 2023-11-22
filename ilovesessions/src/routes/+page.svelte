<script>
    import Header from "../lib/components/Header.svelte";
    import Footer from "../lib/components/Footer.svelte";
</script>

<svelte:head>
    <title>We love web app</title>
</svelte:head>

<Header />

<main>
    <div class="timeline">
        <div class="timeline-item">
          <h4>Event 1: Project Kickoff</h4>
          <p>The project officially begins with a meeting to establish goals, define roles, and outline the timeline.</p>
        </div>
      
        <div class="timeline-item">
          <h4>Event 2: Design Phase Completion</h4>
          <p>The design team finalizes the project's user interface and user experience, ensuring a seamless and intuitive user journey.</p>
        </div>
      
        <div class="timeline-item">
          <h4>Event 3: Development Phase Begins</h4>
          <p>The development team commences coding the project, bringing the design elements to life and implementing the core functionalities.</p>
        </div>
      
        <div class="timeline-item">
          <h4>Event 4: Testing and Bug Fixing</h4>
          <p>Rigorous testing is conducted to identify and resolve any bugs or glitches, ensuring the project's stability and performance.</p>
        </div>
      
        <div class="timeline-item">
          <h4>Event 5: Deployment and Launch</h4>
          <p>The project is successfully deployed and launched, making it accessible to users and marking the culmination of the development journey.</p>
        </div>
      </div>
</main>

<Footer />

<style>
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
</style>