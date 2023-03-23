<template>
  <footer class="container">
    <div class="footer row">
      <div class="col-4">
        <img src="../assets/images/logo.png" alt="Logo" />
        <p class="mt-4 address">
          Jl. Prof. DR. Satrio No.7, RT.3/RW.3, Karet Kuningan, Kecamatan
          Setiabudi, Kota Jakarta Selatan, Daerah Khusus Ibukota Jakarta 12950
        </p>
        <div class="row">
          <div class="col-2">
            <div class="circle">
              <b-icon class="icon" icon="envelope"></b-icon>
            </div>
          </div>
          <div class="col-2">
            <div class="circle">
              <b-icon class="icon" icon="telephone"></b-icon>
            </div>
          </div>
          <div class="col-2">
            <div class="circle">
              <b-icon class="icon" icon="instagram"></b-icon>
            </div>
          </div>
        </div>
      </div>
      <div class="col-2">
        <ul>
          <li class="title">Categories</li>
          <li class="mt-2 list">Cupcake</li>
          <li class="mt-2 list">Pizza</li>
          <li class="mt-2 list">Kebab</li>
          <li class="mt-2 list">Salmon</li>
          <li class="mt-2 list">Doughnut</li>
        </ul>
      </div>
      <div class="col-2">
        <ul>
          <li class="title">About Us</li>
          <li class="mt-2 list">Faq</li>
          <li class="mt-2 list">Kebab</li>
          <li class="mt-2 list">Report Problem</li>
        </ul>
      </div>
      <div class="col-4">
        <ul>
          <li class="title">Newsletter</li>
          <li class="mt-2 list">
            Get now free 50% discount for alll products on your first order
          </li>
          <li class="row mt-2">
            <div class="col-8">
              <input
                class="mr-n3"
                type="email"
                placeholder="Your email address"
              />
            </div>
            <div class="col-2">
              <button class="button button--state-primary">SEND</button>
            </div>
          </li>
          <li class="mt-2 list">
            <b-icon icon="envelope" class="mr-2" style="color: #8bac3e"></b-icon
            >elemesid@gmail.com
          </li>
          <li class="mt-2 list">
            <b-icon
              icon="telephone"
              class="mr-2"
              style="color: #8bac3e"
            ></b-icon
            >0888 1111 2222
          </li>
        </ul>
      </div>
    </div>
    <div class="text-center mt-4">
      <p class="text-copyright">&copy; 2021 Elemes id. All rights reserved</p>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background: #f9fff7;
  border-radius: 20px;
  padding: 74px 62px;
}

.address {
  font-weight: 400;
  font-size: 14px;
  color: #757575;
}

.circle {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #ffffff;
  border-radius: 24px;
  width: 40px;
  height: 40px;
  padding: 10px;
  cursor: pointer;
}

.circle .icon {
  color: #8bac3e;
}

.circle:hover {
  background: #8bac3e;
}

.circle:hover .icon {
  color: #ffffff;
}

ul {
  list-style: none;
}

ul .title {
  font-weight: 500;
  font-size: 18px;
  color: #333333;
  margin-bottom: 33px;
}

ul .list {
  font-weight: 400;
  font-size: 14px;
  color: #757575;
}

input {
  border: 1px solid #000000;
  border-radius: 8px 0 0 8px;
  height: 40px;
  padding: 8px 15px;
}

::placeholder {
  color: #000000;
  font-weight: 400;
  font-size: 14px;
}

.button {
  background: #f2f2f2;
  color: #333333;
  font-weight: 500;
  font-size: 14px;
  padding: 10px 18px;
  height: 40px;
  border-top-right-radius: 8px;
  border-bottom-right-radius: 8px;
  border: none;
}

.button--state-primary {
  background: #8bac3e;
  color: #ffffff;
}

.text-copyright {
  font-weight: 400;
  font-size: 12px;
  text-transform: uppercase;
  color: #757575;
}
</style>
