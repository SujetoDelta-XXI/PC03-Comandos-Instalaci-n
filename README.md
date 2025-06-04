# PC03-Comandos-Instalaci-n

# Github:

git config --global user.name "Tu Nuevo Nombre"
git config --global user.email "tunuevoemail@example.com"

git config --global --list


# React installl:

npm create vite@latest "proyecto"
npm install
npm run dev

# Liberias Install:

npm install react-router-dom
npm install react-toastify
npm install react-loading-skeleton
npm install axios

npm install bootstrap
npm install react-bootstrap bootstrap
//import 'bootstrap/dist/css/bootstrap.min.css';//


#UseDebounce:

import { useState, useEffect } from 'react';

function useDebounce(value, delay) {
  const [debounced, setDebounced] = useState(value);

  useEffect(() => {
    const handler = setTimeout(() => setDebounced(value), delay);
    return () => clearTimeout(handler);
  }, [value, delay]);

  return debounced;
}

export default useDebounce;

