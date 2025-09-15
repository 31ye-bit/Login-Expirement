function addUser() {
  const input = document.getElementById('username');
  const username = input.value.trim();

  if (!username || users.includes(username)) return;

  users.push(username);
  localStorage.setItem('users', JSON.stringify(users));
}
