<script></script>

<template>
  <section class="sectionContact" id="contact">
    <header class="headerContact">
      <h1 class="h1Contact">Contact me</h1>
    </header>
    <div class="generalContact">
      <div class="container1">
        <header class="header2">
          <h2 class="h2">Contact with me</h2>
          <p class="phrase1">
            I'm open to new opportunities and collaborations. Follow me or get
            in touch!
          </p>
        </header>
        <div class="divContacts">
          <p class="pInfoP">
            <i class="fa-solid fa-envelope iconsContact"></i
            >@norkysgabrielasanchezreyes@gmail.com
          </p>
          <p class="pInfoP">
            <i class="fa-solid fa-phone iconsContact"></i>809-974-9584
          </p>
          <p class="pInfoP">
            <i class="fa-solid fa-location-dot iconsContact"></i>Dominican
            Republic. Santo Domingo
          </p>
        </div>
        <div class="imgsContact">
          <a
            href="https://www.instagram.com/gabxyys?igsh=MWxkNXR6MHhwbWRucA%3D%3D&utm_source=qr"
          >
            <img class="imgIconsContact" src="../assets/svg/Instagram.svg" />
          </a>
          <a
            href="https://www.linkedin.com/in/norkys-gabriela-sanchez-reyes-643947362"
          >
            <img class="imgIconsContactLk" src="../assets/svg/Linkedin.svg" />
          </a>
          <a href="https://www.facebook.com/DR.BSalltheway?mibextid=LQQJ4d">
            <img class="imgIconsContactFc" src="../assets/svg/Facebook.svg" />
          </a>
          <a href="https://x.com/Shellsss00">
            <img class="imgIconsContactFc" src="../assets/svg/Twitter.svg" />
          </a>
        </div>
      </div>
      <div class="container2">
        <header class="header3">
          <h3 class="h2">Send a Message</h3>
          <p class="phrase2">
            Do you have an idea or project in mind? <br />Tell me in a message
            and let's make it happen!
          </p>
        </header>
        <form class="form">
          <input type="text" class="inputs" placeholder="Name" />
          <input type="email" class="inputs" placeholder="Email" />
          <textarea class="inputMessage" placeholder="Message"></textarea>
        </form>
        <button class="btnSend">
          Send <i class="fa-solid fa-paper-plane iconSend"></i>
        </button>
      </div>
    </div>
  </section>
</template>

<style scoped>
.sectionContact {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #050505;
  width: 100%;
  height: 600px;
  gap: 30px;
}

.generalContact {
  display: flex;
  gap: 60px;
}

.header3 {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.divForm {
  width: 490px;
  height: 350px;
  box-shadow: 0 4px 15px rgba(155, 48, 255, 0.3);
  border-radius: 10px;
}

.h1Contact {
  color: #a855f7;
  font-family: "Poppins", system-ui;
}

.divContacts {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.header2 {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.generalContact {
  display: flex;
  justify-content: center;
  align-items: center;
}

.container1 {
  display: flex;
  flex-direction: column;
  gap: 30px;
}

.h2 {
  color: #fff;
  font-family: "Poppins", system-ui;
}

.phrase1 {
  color: #fff;
  font-family: "Poppins", system-ui;
}

.phrase2 {
  color: #fff;
  font-family: "Poppins", system-ui;
}

.pInfoP {
  color: #fff;
  display: flex;
  gap: 10px;
}

.iconsContact {
  color: #a855f7;
}

.imgsContact {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
}

.imgIconsContactLk {
  width: 41px;
}

.imgIconsContact {
  width: 36px;
}

.imgIconsContactFc {
  width: 41px;
}

.container2 {
  display: flex;
  flex-direction: column;
  gap: 40px;
  width: 500px;
  height: 460px;
  justify-content: center;
}

.form {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.inputs {
  width: 200px;
  height: 32px;
  border-radius: 8px;
  padding: 13px;
  border: none;
  outline: none;
  font-family: "Poppins", system-ui;
}

.inputMessage {
  width: 390px;
  height: 100px;
  padding: 13px;
  font-family: "Poppins", system-ui;
  outline: none;
  border-radius: 8px;
}

.btnSend {
  width: 120px;
  height: 30px;
  border: none;
  border-radius: 5px;
  font-weight: bold;
  cursor: pointer;
  transition: 0.3s ease;
  border: solid 1px #a855f7;
  box-shadow: 0 0 25px #a855f7;
  background-color: #a855f7;
  color: #fff;
}

.btnSend:hover {
  transform: scale(1.1);
}

.iconSend {
  color: #fff;
}

@media (max-width: 768px) {
  .sectionContact {
    height: 100%;
  }

  .generalContact {
    flex-direction: column;
  }

  .divContacts {
    justify-content: center;
    align-items: center;
  }

  .header2 {
    justify-content: center;
    align-items: center;
  }

  .phrase1 {
    width: 300px;
    text-align: center;
  }

  .container2 {
    justify-content: center;
    align-items: center;
  }
}
</style>
