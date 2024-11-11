<script setup></script>

<template>
  <div class="form-container">
    <form class="form">
      <div class="form-group">
        <input type="text" placeholder="Nombre completo" />
        <input
          required=""
          name="email"
          id="email"
          placeholder="Email"
          type="text"
        />
      </div>
      <div class="form-group">
        <label for="textarea">¿Cómo puedo ayudarte?</label>
        <textarea required="" cols="50" rows="10" id="textarea" name="textarea">
        </textarea>
      </div>
      <button type="submit" class="form-submit-btn">Enviar</button>
    </form>
  </div>
</template>

<style scoped>
.form-container {
  width: 400px;
  background: linear-gradient(#212121, #212121) padding-box,
    linear-gradient(145deg, transparent 35%, #36a8fa, #ff0f7b) border-box;
  border: 2px solid transparent;
  padding: 32px 24px;
  font-size: 14px;
  font-family: inherit;
  color: white;
  display: flex;
  flex-direction: column;
  gap: 20px;
  box-sizing: border-box;
  border-radius: 16px;
  background-size: 200% 100%;
  animation: gradient 5s ease infinite;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }

  50% {
    background-position: 100% 50%;
  }

  100% {
    background-position: 0% 50%;
  }
}

.form-container button:active {
  scale: 0.95;
}

.form-container .form {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.form-container .form-group {
  display: flex;
  flex-direction: column;
  gap: 2px;
}

.form-container .form-group label {
  display: block;
  margin-bottom: 5px;
  color: #717171;
  font-weight: 600;
  font-size: 12px;
}

.form-container .form-group input {
  width: 100%;
  padding: 12px 16px;
  border-radius: 8px;
  color: #fff;
  font-family: inherit;
  background-color: transparent;
  border: 1px solid #414141;
}

.form-container .form-group textarea {
  width: 100%;
  padding: 12px 16px;
  border-radius: 8px;
  resize: none;
  color: #fff;
  height: 96px;
  border: 1px solid #414141;
  background-color: transparent;
  font-family: inherit;
}

.form-container .form-group input::placeholder {
  opacity: 0.5;
}

.form-container .form-group input:focus {
  outline: none;
  border-color: #ff0f7b;
}

.form-container .form-group textarea:focus {
  outline: none;
  border-color: #36a8fa;
}

.form-container .form-submit-btn {
  display: flex;
  align-items: flex-start;
  justify-content: center;
  align-self: flex-start;
  font-family: inherit;
  color: white;
  font-weight: 600;
  width: 40%;
  background: #313131;
  border: 1px solid #414141;
  padding: 12px 16px;
  font-size: inherit;
  gap: 8px;
  margin-top: 8px;
  cursor: pointer;
  border-radius: 6px;
}

.form-container .form-submit-btn:hover {
  background: linear-gradient(45deg, #36a8fa, #ff0f7b);
}
</style>
