<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Live Currency Converter</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        .animate-spin {
            animation: spin 1s linear infinite;
        }
    </style>
</head>
<body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-screen p-8">
    <div class="max-w-4xl mx-auto">
        <div class="bg-white rounded-2xl shadow-xl p-8">
            <!-- Header -->
            <div class="flex items-center justify-between mb-6">
                <div class="flex items-center gap-3">
                    <div class="bg-indigo-600 p-3 rounded-xl">
                        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                        </svg>
                    </div>
                    <div>
                        <h1 class="text-3xl font-bold text-gray-800">Currency Converter</h1>
                        <p class="text-gray-600" id="lastUpdate">Loading rates...</p>
                    </div>
                </div>
                <button
                    onclick="fetchRates()"
                    id="refreshBtn"
                    class="bg-indigo-600 hover:bg-indigo-700 text-white px-4 py-2 rounded-lg font-medium flex items-center gap-2 transition"
                >
                    <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15"></path>
                    </svg>
                    Refresh
                </button>
            </div>

            <!-- Amount Input -->
            <div class="mb-8">
                <label class="block text-sm font-medium text-gray-700 mb-2">Enter Amount</label>
                <input
                    type="number"
                    id="amount"
                    value="100"
                    oninput="convertAll()"
                    class="w-full px-6 py-4 border-2 border-indigo-300 rounded-xl focus:ring-2 focus:ring-indigo-500 focus:border-indigo-500 outline-none transition text-3xl font-bold text-center"
                    placeholder="0.00"
                />
            </div>
    
            <!-- Currency Cards -->
            <div class="grid md:grid-cols-2 gap-4">
                <!-- PLN -->
                <div class="bg-gradient-to-br from-indigo-50 to-blue-50 p-6 rounded-xl border-2 border-indigo-200 hover:border-indigo-400 transition cursor-pointer" onclick="setActiveCurrency('PLN')">
                    <div class="flex items-center justify-between mb-3">
                        <div class="flex items-center gap-3">
                            <span class="text-4xl">🇵🇱</span>
                            <div>
                                <h3 class="text-xl font-bold text-gray-800">PLN</h3>
                                <p class="text-sm text-gray-600">Polish Złoty</p>
                            </div>
                        </div>
                    </div>
                    <div class="text-right">
                        <p class="text-3xl font-bold text-indigo-700" id="amount-PLN">100.00</p>
                        <p class="text-sm text-gray-600 mt-1">zł</p>
                    </div>
                </div>
    
                <!-- USD -->
                <div class="bg-gradient-to-br from-indigo-50 to-blue-50 p-6 rounded-xl border-2 border-indigo-200 hover:border-indigo-400 transition cursor-pointer" onclick="setActiveCurrency('USD')">
                    <div class="flex items-center justify-between mb-3">
                        <div class="flex items-center gap-3">
                            <span class="text-4xl">🇺🇸</span>
                            <div>
                                <h3 class="text-xl font-bold text-gray-800">USD</h3>
                                <p class="text-sm text-gray-600">US Dollar</p>
                            </div>
                        </div>
                    </div>
                    <div class="text-right">
                        <p class="text-3xl font-bold text-indigo-700" id="amount-USD">0.00</p>
                        <p class="text-sm text-gray-600 mt-1">$</p>
                    </div>
                </div>
    
                <!-- EUR -->
                <div class="bg-gradient-to-br from-indigo-50 to-blue-50 p-6 rounded-xl border-2 border-indigo-200 hover:border-indigo-400 transition cursor-pointer" onclick="setActiveCurrency('EUR')">
                    <div class="flex items-center justify-between mb-3">
                        <div class="flex items-center gap-3">
                            <span class="text-4xl">🇪🇺</span>
                            <div>
                                <h3 class="text-xl font-bold text-gray-800">EUR</h3>
                                <p class="text-sm text-gray-600">Euro</p>
                            </div>
                        </div>
                    </div>
                    <div class="text-right">
                        <p class="text-3xl font-bold text-indigo-700" id="amount-EUR">0.00</p>
                        <p class="text-sm text-gray-600 mt-1">€</p>
                    </div>
                </div>
    
                <!-- CHF -->
                <div class="bg-gradient-to-br from-indigo-50 to-blue-50 p-6 rounded-xl border-2 border-indigo-200 hover:border-indigo-400 transition cursor-pointer" onclick="setActiveCurrency('CHF')">
                    <div class="flex items-center justify-between mb-3">
                        <div class="flex items-center gap-3">
                            <span class="text-4xl">🇨🇭</span>
                            <div>
                                <h3 class="text-xl font-bold text-gray-800">CHF</h3>
                                <p class="text-sm text-gray-600">Swiss Franc</p>
                            </div>
                        </div>
                    </div>
                    <div class="text-right">
                        <p class="text-3xl font-bold text-indigo-700" id="amount-CHF">0.00</p>
                        <p class="text-sm text-gray-600 mt-1">Fr</p>
                    </div>
                </div>
            </div>
    
            <!-- Exchange Rates Reference -->
            <div class="mt-8 border-t border-gray-200 pt-6">
                <h3 class="text-sm font-semibold text-gray-700 mb-3">Current Exchange Rates (Base: 1 PLN)</h3>
                <div class="grid grid-cols-3 gap-3">
                    <div class="bg-indigo-50 p-3 rounded-lg text-center">
                        <p class="text-xs text-gray-600">PLN → USD</p>
                        <p class="text-lg font-bold text-indigo-700" id="rate-USD">-</p>
                    </div>
                    <div class="bg-indigo-50 p-3 rounded-lg text-center">
                        <p class="text-xs text-gray-600">PLN → EUR</p>
                        <p class="text-lg font-bold text-indigo-700" id="rate-EUR">-</p>
                    </div>
                    <div class="bg-indigo-50 p-3 rounded-lg text-center">
                        <p class="text-xs text-gray-600">PLN → CHF</p>
                        <p class="text-lg font-bold text-indigo-700" id="rate-CHF">-</p>
                    </div>
                </div>
            </div>
    
            <!-- Info Note -->
            <div class="mt-6 p-4 bg-blue-50 border border-blue-200 rounded-lg">
                <p class="text-sm text-blue-800">
                    <strong>💡 Tip:</strong> Type any amount and see instant conversions to all currencies. Rates update automatically every 60 seconds.
                </p>
            </div>
        </div>
    </div>
    
    <script>
        let rates = {};
        let activeCurrency = 'PLN';
        const currencies = ['PLN', 'USD', 'EUR', 'CHF'];
    
        async function fetchRates() {
            const refreshBtn = document.getElementById('refreshBtn');
            const lastUpdate = document.getElementById('lastUpdate');
            
            refreshBtn.disabled = true;
            refreshBtn.innerHTML = `
                <svg class="animate-spin w-5 h-5" fill="none" viewBox="0 0 24 24">
                    <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                    <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
                </svg>
                Updating...
            `;
    
            try {
                const response = await fetch('https://api.exchangerate-api.com/v4/latest/PLN');
                const data = await response.json();
                
                rates = {
                    PLN: 1,
                    USD: data.rates.USD,
                    EUR: data.rates.EUR,
                    CHF: data.rates.CHF
                };
    
                const now = new Date();
                lastUpdate.textContent = `Updated: ${now.toLocaleTimeString()}`;
                
                displayRates();
                convertAll();
            } catch (error) {
                console.error('Error fetching rates:', error);
                lastUpdate.textContent = 'Error loading rates. Click refresh.';
            }
    
            refreshBtn.disabled = false;
            refreshBtn.innerHTML = `
                <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15"></path>
                </svg>
                Refresh
            `;
        }
    
        function displayRates() {
            document.getElementById('rate-USD').textContent = rates.USD.toFixed(4);
            document.getElementById('rate-EUR').textContent = rates.EUR.toFixed(4);
            document.getElementById('rate-CHF').textContent = rates.CHF.toFixed(4);
        }
    
        function setActiveCurrency(currency) {
            activeCurrency = currency;
            convertAll();
        }
    
        function convertRate(amount, from, to) {
            const inPLN = amount / rates[from];
            return inPLN * rates[to];
        }
    
        function convertAll() {
            const inputAmount = parseFloat(document.getElementById('amount').value) || 0;
    
            if (Object.keys(rates).length === 0) {
                return;
            }
    
            currencies.forEach(currency => {
                const result = convertRate(inputAmount, activeCurrency, currency);
                document.getElementById(`amount-${currency}`).textContent = result.toFixed(2);
            });
        }
    
        // Fetch rates on load
        fetchRates();
    
        // Auto-refresh every 60 seconds
        setInterval(fetchRates, 60000);
    </script>
</body>
</html>