<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zaid Furniture | Premium Store</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root { --primary-color: #5d4037; }
        .theme-bg { background-color: var(--primary-color); }
        .theme-text { color: var(--primary-color); }
        .theme-border { border-color: var(--primary-color); }
        .cart-badge { position: absolute; top: -8px; right: -12px; background: #ef4444; color: white; border-radius: 50%; padding: 2px 7px; font-size: 11px; font-weight: bold; }
    </style>
</head>
<body class="bg-gray-50 font-sans text-gray-900">

    <!-- Navbar -->
    <nav class="theme-bg text-white sticky top-0 z-50 shadow-lg">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <div>
                <h1 id="displayBrandName" class="text-2xl font-black tracking-tight uppercase">Zaid Furniture</h1>
                <p id="displayAddress" class="text-[10px] opacity-80"></p>
            </div>
            <div class="flex items-center gap-8">
                <button onclick="toggleCart()" class="relative hover:scale-110 transition">
                    <i class="fa-solid fa-bag-shopping text-2xl"></i>
                    <span id="cartCount" class="cart-badge">0</span>
                </button>
                <button onclick="toggleAdmin()" class="bg-white/20 hover:bg-white/30 p-2 rounded-lg transition">
                    <i class="fa-solid fa-gears"></i>
                </button>
            </div>
        </div>
    </nav>

    <!-- Main Storefront -->
    <main class="container mx-auto px-6 py-10">
        <div id="productGrid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
            <!-- Products Loaded Dynamically -->
        </div>
    </main>

    <!-- Cart Sidebar -->
    <div id="cartModal" class="fixed inset-0 bg-black/60 hidden z-[100] flex justify-end backdrop-blur-sm">
        <div class="bg-white w-full max-w-md h-full shadow-2xl flex flex-col animate-in slide-in-from-right duration-300">
            <div class="p-6 border-b flex justify-between items-center bg-gray-50">
                <h2 class="text-xl font-bold">Shopping Cart</h2>
                <button onclick="toggleCart()" class="text-3xl">&times;</button>
            </div>
            <div id="cartItems" class="flex-1 overflow-y-auto p-6 space-y-4"></div>
            <div class="p-6 border-t bg-gray-50">
                <div class="flex justify-between text-xl font-bold mb-6">
                    <span>Total Amount:</span>
                    <span class="theme-text">₹<span id="totalPrice">0</span></span>
                </div>
                <button onclick="openCheckout()" class="w-full bg-green-600 text-white py-4 rounded-2xl font-bold text-lg hover:bg-green-700 transition shadow-lg">
                    <i class="fa-brands fa-whatsapp mr-2"></i> Checkout via WhatsApp
                </button>
            </div>
        </div>
    </div>

    <!-- Admin Panel -->
    <div id="adminPanel" class="fixed inset-0 bg-black/70 hidden z-[200] flex items-center justify-center p-4">
        <div class="bg-white w-full max-w-2xl rounded-3xl shadow-2xl max-h-[90vh] overflow-y-auto">
            <div class="p-6 border-b flex justify-between items-center bg-slate-100">
                <h2 class="text-xl font-black uppercase">Store Control Panel</h2>
                <button onclick="toggleAdmin()" class="text-2xl">&times;</button>
            </div>
            
            <div class="p-8 space-y-8">
                <!-- Shop Settings -->
                <section>
                    <h3 class="font-bold text-blue-600 mb-4 border-b pb-2"><i class="fa-solid fa-shop mr-2"></i>Shop Profile</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <input type="text" id="editShopName" placeholder="Shop Name" class="border p-3 rounded-xl outline-none">
                        <input type="text" id="editPhone" placeholder="WhatsApp (e.g. 919050388349)" class="border p-3 rounded-xl outline-none">
                        <input type="color" id="editColor" class="w-full h-12 rounded-xl cursor-pointer border">
                        <input type="text" id="editAddress" placeholder="Shop Address" class="border p-3 rounded-xl outline-none">
                    </div>
                </section>

                <!-- Inventory Management -->
                <section>
                    <h3 class="font-bold text-orange-600 mb-4 border-b pb-2"><i class="fa-solid fa-plus mr-2"></i>Add Product</h3>
                    <div class="space-y-3">
                        <input type="text" id="newTitle" placeholder="Product Title" class="w-full border p-3 rounded-xl">
                        <input type="number" id="newPrice" placeholder="Price (₹)" class="w-full border p-3 rounded-xl">
                        <textarea id="newDesc" placeholder="Description" class="w-full border p-3 rounded-xl"></textarea>
                        <input type="file" id="newImg" class="w-full text-sm">
                    </div>
                </section>
            </div>

            <div class="p-6 border-t flex gap-4">
                <button onclick="saveAdminSettings()" class="bg-blue-600 text-white flex-1 py-4 rounded-2xl font-bold hover:bg-blue-700 shadow-lg transition">Apply All Changes</button>
            </div>
        </div>
    </div>

    <!-- Checkout Modal -->
    <div id="checkoutModal" class="fixed inset-0 bg-black/80 hidden z-[300] flex items-center justify-center p-4">
        <div class="bg-white p-8 rounded-3xl w-full max-w-md">
            <h2 class="text-2xl font-bold mb-6">Delivery Details</h2>
            <div class="space-y-4">
                <input type="text" id="custName" placeholder="Full Name" class="w-full border-2 p-3 rounded-xl">
                <input type="number" id="custPhone" placeholder="Mobile Number" class="w-full border-2 p-3 rounded-xl">
                <textarea id="custAddr" placeholder="Full Address" class="w-full border-2 p-3 rounded-xl"></textarea>
                <button onclick="confirmAndSend()" class="w-full bg-green-600 text-white py-4 rounded-xl font-bold text-lg">Send Order Now</button>
            </div>
        </div>
    </div>

    <script>
        // Default Configuration
        const defaultConfig = {
            shopName: "Zaid Furniture",
            phone: "919050388349",
            address: "Main Market Tauru, Nuh, Haryana 122105",
            color: "#5d4037",
            products: [
                { id: 1, title: "Royal King Bed", price: 28000, desc: "Premium Woodwork", img: "https://via.placeholder.com/300" }
            ]
        };

        let storeData = JSON.parse(localStorage.getItem('zaidStoreData')) || defaultConfig;
        let cart = [];

        function renderStore() {
            // Update Branding
            document.getElementById('displayBrandName').innerText = storeData.shopName;
            document.getElementById('displayAddress').innerText = storeData.address;
            document.documentElement.style.setProperty('--primary-color', storeData.color);

            // Update Products
            const grid = document.getElementById('productGrid');
            grid.innerHTML = storeData.products.map(p => `
                <div class="bg-white rounded-3xl overflow-hidden shadow-sm hover:shadow-xl transition-all border border-gray-100 group">
                    <img src="${p.img}" class="w-full h-48 object-cover group-hover:scale-105 transition duration-500">
                    <div class="p-5">
                        <h4 class="font-bold text-lg mb-1">${p.title}</h4>
                        <p class="text-gray-500 text-sm mb-3 line-clamp-1">${p.desc}</p>
                        <div class="flex justify-between items-center">
                            <span class="text-xl font-black theme-text">₹${p.price}</span>
                            <button onclick="addToCart(${p.id})" class="bg-orange-500 text-white px-4 py-2 rounded-xl font-bold text-sm hover:bg-orange-600 transition shadow-md">Add</button>
                        </div>
                    </div>
                </div>
            `).join('');
        }

        function addToCart(id) {
            const product = storeData.products.find(p => p.id === id);
            cart.push(product);
            updateCartUI();
        }

        function updateCartUI() {
            document.getElementById('cartCount').innerText = cart.length;
            const container = document.getElementById('cartItems');
            let total = 0;
            container.innerHTML = cart.map((item, index) => {
                total += item.price;
                return `
                <div class="flex justify-between items-center bg-gray-100 p-4 rounded-2xl">
                    <div><p class="font-bold">${item.title}</p><p class="text-sm opacity-70">₹${item.price}</p></div>
                    <button onclick="removeFromCart(${index})" class="text-red-500"><i class="fa-solid fa-trash"></i></button>
                </div>`;
            }).join('');
            document.getElementById('totalPrice').innerText = total;
        }

        function removeFromCart(index) {
            cart.splice(index, 1);
            updateCartUI();
        }

        function saveAdminSettings() {
            storeData.shopName = document.getElementById('editShopName').value || storeData.shopName;
            storeData.phone = document.getElementById('editPhone').value || storeData.phone;
            storeData.address = document.getElementById('editAddress').value || storeData.address;
            storeData.color = document.getElementById('editColor').value;

            const newTitle = document.getElementById('newTitle').value;
            const newPrice = document.getElementById('newPrice').value;
            const newDesc = document.getElementById('newDesc').value;
            const newImgFile = document.getElementById('newImg').files[0];

            if(newTitle && newPrice) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    storeData.products.unshift({ id: Date.now(), title: newTitle, price: parseInt(newPrice), desc: newDesc, img: e.target.result });
                    finalizeSave();
                };
                if(newImgFile) reader.readAsDataURL(newImgFile);
                else {
                    storeData.products.unshift({ id: Date.now(), title: newTitle, price: parseInt(newPrice), desc: newDesc, img: "https://via.placeholder.com/300" });
                    finalizeSave();
                }
            } else {
                finalizeSave();
            }
        }

        function finalizeSave() {
            localStorage.setItem('zaidStoreData', JSON.stringify(storeData));
            renderStore();
            toggleAdmin();
            alert("Settings Saved Successfully!");
        }

        function confirmAndSend() {
            const name = document.getElementById('custName').value;
            const phone = document.getElementById('custPhone').value;
            const addr = document.getElementById('custAddr').value;

            if(!name || !phone || !addr) return alert("Please fill all details!");

            let message = `*ZAID FURNITURE - NEW ORDER*%0A%0A`;
            message += `*Customer:* ${name}%0A*Phone:* ${phone}%0A*Address:* ${addr}%0A%0A*Items Ordered:*%0A`;
            cart.forEach(item => message += `- ${item.title} (₹${item.price})%0A`);
            message += `%0A*Grand Total: ₹${document.getElementById('totalPrice').innerText}*%0A%0A*Shop:* ${storeData.shopName}%0A*Loc:* ${storeData.address}`;

            window.open(`https://wa.me/${storeData.phone}?text=${message}`, '_blank');
            cart = [];
            updateCartUI();
            document.getElementById('checkoutModal').classList.add('hidden');
            toggleCart();
        }

        function toggleAdmin() {
            document.getElementById('adminPanel').classList.toggle('hidden');
            document.getElementById('editShopName').value = storeData.shopName;
            document.getElementById('editPhone').value = storeData.phone;
            document.getElementById('editAddress').value = storeData.address;
            document.getElementById('editColor').value = storeData.color;
        }

        function toggleCart() { document.getElementById('cartModal').classList.toggle('hidden'); }
        function openCheckout() { if(cart.length > 0) document.getElementById('checkoutModal').classList.remove('hidden'); }

        renderStore();
    </script>
</body>
</html>
