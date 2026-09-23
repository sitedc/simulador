
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simulação de Crédito Rápido | R$ 1 MIL a R$ 10 MIL+</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            100: '#dcfce7',
                            500: '#22c55e',
                            600: '#16a34a',
                            700: '#15803d',
                            800: '#166534',
                            900: '#14532d',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-bg {
            background: linear-gradient(135deg, #020617 0%, #0f172a 50%, #14532d 100%);
        }
        .card-glow {
            box-shadow: 0 10px 30px -10px rgba(34, 197, 94, 0.25);
        }
        @keyframes pulse-slow {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.85; transform: scale(1.03); }
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans antialiased selection:bg-brand-500 selection:text-white pb-16 md:pb-0">

    <!-- TOP ANNOUNCEMENT BAR -->
    <div class="bg-brand-600 text-white text-xs md:text-sm font-semibold py-2 px-4 text-center tracking-wide shadow-inner">
        <i class="fa-solid fa-bolt mr-2 text-yellow-300"></i>
        LIBERAÇÃO RÁPIDA VIA PIX • ATENDIMENTO PARA TODO O BRASIL
    </div>

    <!-- MAIN HEADER -->
    <header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md border-b border-slate-200 transition-all shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- LOGO -->
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-brand-700 to-brand-500 flex items-center justify-center text-white font-extrabold text-xl shadow-md">
                    <i class="fa-solid fa-hand-holding-dollar"></i>
                </div>
                <div>
                    <span class="text-xl md:text-2xl font-black text-slate-900 tracking-tight">CRÉDITO<span class="text-brand-600">FÁCIL</span></span>
                    <span class="block text-[10px] text-slate-500 font-medium tracking-wider uppercase">Soluções Financeiras</span>
                </div>
            </div>

            <!-- DESKTOP CONTACT BUTTONS -->
            <div class="hidden md:flex items-center gap-6">
                <div class="flex items-center gap-2 text-slate-600 text-sm font-medium">
                    <i class="fa-solid fa-shield-halved text-brand-600 text-lg"></i>
                    <span>Correspondente Autorizado</span>
                </div>
                <a href="#simulador" class="inline-flex items-center justify-center px-5 py-2.5 rounded-full text-sm font-bold text-white bg-brand-600 hover:bg-brand-700 transition duration-200 shadow-md hover:shadow-lg">
                    <i class="fa-solid fa-calculator mr-2"></i> Simular Agora
                </a>
            </div>
        </div>
    </header>

    <!-- HERO SECTION WITH INTEGRATED FORM -->
    <section class="relative gradient-bg text-white py-12 md:py-20 overflow-hidden">
        <div class="absolute -top-24 -left-24 w-96 h-96 bg-brand-500/10 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-0 right-0 w-96 h-96 bg-brand-500/15 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                
                <!-- HERO LEFT CONTENT -->
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 bg-slate-800/80 border border-slate-700/80 px-4 py-2 rounded-full text-xs md:text-sm font-semibold text-brand-500 shadow-sm">
                        <span class="w-2 h-2 rounded-full bg-brand-500 animate-ping"></span>
                        Simulação 100% Gratuita e Sem Burocracia
                    </div>

                    <h1 class="text-3xl sm:text-4xl lg:text-5xl font-black leading-tight tracking-tight">
                        Crédito e Benefícios de <br class="hidden sm:inline">
                        <span class="text-transparent bg-clip-text bg-gradient-to-r from-brand-500 via-green-300 to-emerald-400">
                            R$ 1.000 a R$ 10.000+
                        </span>
                    </h1>

                    <p class="text-slate-300 text-base sm:text-lg max-w-2xl mx-auto lg:mx-0 leading-relaxed">
                        Atendimento exclusivo e crédito facilitado para <strong class="text-white">Aposentados, Pensionistas, Servidores Públicos (Estaduais e Federais), Trabalhadores CLT e Forças Armadas</strong>.
                    </p>

                    <!-- QUICK VALUE CHIPS -->
                    <div class="pt-2">
                        <p class="text-xs font-semibold uppercase tracking-wider text-slate-400 mb-3">Selecione ou consulte o valor pretendido:</p>
                        <div class="flex flex-wrap justify-center lg:justify-start gap-2 sm:gap-3">
                            <button type="button" onclick="selectQuickValue('1000')" class="chip-val bg-slate-800/90 border border-slate-700 hover:border-brand-500 text-brand-500 font-bold px-4 py-2 rounded-xl text-sm transition flex items-center gap-2">
                                <i class="fa-solid fa-coins"></i> R$ 1 MIL
                            </button>
                            <button type="button" onclick="selectQuickValue('3000')" class="chip-val bg-slate-800/90 border border-slate-700 hover:border-brand-500 text-brand-500 font-bold px-4 py-2 rounded-xl text-sm transition flex items-center gap-2">
                                <i class="fa-solid fa-money-bill-wave"></i> R$ 3 MIL
                            </button>
                            <button type="button" onclick="selectQuickValue('5000')" class="chip-val bg-slate-800/90 border border-slate-700 hover:border-brand-500 text-brand-500 font-bold px-4 py-2 rounded-xl text-sm transition flex items-center gap-2">
                                <i class="fa-solid fa-wallet"></i> R$ 5 MIL
                            </button>
                            <button type="button" onclick="selectQuickValue('10000')" class="chip-val bg-slate-800/90 border border-slate-700 hover:border-brand-500 text-brand-500 font-bold px-4 py-2 rounded-xl text-sm transition flex items-center gap-2">
                                <i class="fa-solid fa-sack-dollar"></i> R$ 10 MIL+
                            </button>
                        </div>
                    </div>

                    <!-- TRUST BADGES HERO -->
                    <div class="pt-4 grid grid-cols-3 gap-4 border-t border-slate-800 text-center max-w-lg mx-auto lg:mx-0">
                        <div>
                            <div class="text-xl sm:text-2xl font-black text-white">98%</div>
                            <div class="text-xs text-slate-400">Taxa de Aprovados</div>
                        </div>
                        <div>
                            <div class="text-xl sm:text-2xl font-black text-white">PIX</div>
                            <div class="text-xs text-slate-400">Receba Direto</div>
                        </div>
                        <div>
                            <div class="text-xl sm:text-2xl font-black text-white">100%</div>
                            <div class="text-xs text-slate-400">Seguro e Digital</div>
                        </div>
                    </div>
                </div>

                <!-- HERO RIGHT LEAD FORM -->
                <div id="simulador" class="lg:col-span-5">
                    <div class="bg-white text-slate-800 rounded-3xl p-6 sm:p-8 shadow-2xl card-glow relative border border-slate-100">
                        <div class="absolute -top-3 right-6 bg-brand-500 text-white text-[11px] font-black uppercase px-3 py-1 rounded-full shadow-sm tracking-wider">
                            Atendimento Prioritário
                        </div>

                        <h2 class="text-2xl font-extrabold text-slate-900 mb-1">Simule Seu Crédito</h2>
                        <p class="text-slate-500 text-xs mb-6">Preencha seus dados para receber o atendimento no WhatsApp.</p>

                        <form id="leadForm" onsubmit="handleFormSubmit(event)" class="space-y-4">
                            
                            <!-- PERFIL SELECTOR BUTTONS -->
                            <div>
                                <label class="block text-xs font-bold text-slate-700 uppercase tracking-wider mb-2">
                                    Selecione seu Perfil <span class="text-red-500">*</span>
                                </label>
                                <div class="grid grid-cols-2 gap-2" id="profileGrid">
                                    <button type="button" onclick="selectProfile('Aposentado/Pensionista')" class="profile-btn border-2 border-slate-200 hover:border-brand-500 bg-slate-50 p-2.5 rounded-xl text-left text-xs font-bold text-slate-700 flex items-center gap-2 transition">
                                        <i class="fa-solid fa-hands-holding-circle text-brand-600 text-base"></i>
                                        <span>Aposentado / Pensionista</span>
                                    </button>
                                    <button type="button" onclick="selectProfile('Servidor Público')" class="profile-btn border-2 border-slate-200 hover:border-brand-500 bg-slate-50 p-2.5 rounded-xl text-left text-xs font-bold text-slate-700 flex items-center gap-2 transition">
                                        <i class="fa-solid fa-building-columns text-brand-600 text-base"></i>
                                        <span>Servidor Público (Estadual/Federal)</span>
                                    </button>
                                    <button type="button" onclick="selectProfile('Trabalhador CLT')" class="profile-btn border-2 border-slate-200 hover:border-brand-500 bg-slate-50 p-2.5 rounded-xl text-left text-xs font-bold text-slate-700 flex items-center gap-2 transition">
                                        <i class="fa-solid fa-briefcase text-brand-600 text-base"></i>
                                        <span>Trabalhador CLT</span>
                                    </button>
                                    <button type="button" onclick="selectProfile('Forças Armadas')" class="profile-btn border-2 border-slate-200 hover:border-brand-500 bg-slate-50 p-2.5 rounded-xl text-left text-xs font-bold text-slate-700 flex items-center gap-2 transition">
                                        <i class="fa-solid fa-shield-halved text-brand-600 text-base"></i>
                                        <span>Forças Armadas</span>
                                    </button>
                                </div>
                                <input type="hidden" id="selectedProfile" name="perfil" required>
                                <p id="profileError" class="text-red-500 text-[11px] mt-1 hidden">Por favor, selecione seu perfil acima.</p>
                            </div>

                            <!-- VALOR DESEJADO SELECTOR -->
                            <div>
                                <label for="valorDesejado" class="block text-xs font-bold text-slate-700 uppercase tracking-wider mb-1">
                                    Valor Desejado <span class="text-red-500">*</span>
                                </label>
                                <div class="relative">
                                    <div class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400 font-bold">
                                        R$
                                    </div>
                                    <select id="valorDesejado" name="valor" class="w-full pl-11 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-brand-500 focus:border-brand-500 text-slate-800 font-bold text-sm bg-slate-50">
                                        <option value="1000">1.000,00 (Um Mil Reais)</option>
                                        <option value="3000" selected>3.000,00 (Três Mil Reais)</option>
                                        <option value="5000">5.000,00 (Cinco Mil Reais)</option>
                                        <option value="10000">10.000,00 ou Mais</option>
                                    </select>
                                </div>
                            </div>

                            <!-- NOME COMPLETO -->
                            <div>
                                <label for="fullName" class="block text-xs font-bold text-slate-700 uppercase tracking-wider mb-1">
                                    Nome Completo <span class="text-red-500">*</span>
                                </label>
                                <div class="relative">
                                    <div class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
                                        <i class="fa-regular fa-user"></i>
                                    </div>
                                    <input type="text" id="fullName" name="nome" placeholder="Digite seu nome completo" required
                                        class="w-full pl-10 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-brand-500 focus:border-brand-500 text-sm bg-slate-50">
                                </div>
                            </div>

                            <!-- CPF FORM FIELD -->
                            <div>
                                <label for="cpf" class="block text-xs font-bold text-slate-700 uppercase tracking-wider mb-1">
                                    CPF do Titular <span class="text-red-500">*</span>
                                </label>
                                <div class="relative">
                                    <div class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
                                        <i class="fa-regular fa-id-card"></i>
                                    </div>
                                    <input type="text" id="cpf" name="cpf" placeholder="000.000.000-00" maxlength="14" required
                                        oninput="maskCPF(this)"
                                        class="w-full pl-10 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-brand-500 focus:border-brand-500 text-sm font-semibold tracking-wider bg-slate-50">
                                </div>
                                <span class="text-[10px] text-slate-400 flex items-center gap-1 mt-1">
                                    <i class="fa-solid fa-lock text-[9px]"></i> Seus dados estão seguros e protegidos pela LGPD.
                                </span>
                            </div>

                            <!-- WHATSAPP FIELD -->
                            <div>
                                <label for="phone" class="block text-xs font-bold text-slate-700 uppercase tracking-wider mb-1">
                                    WhatsApp para Contato <span class="text-red-500">*</span>
                                </label>
                                <div class="relative">
                                    <div class="absolute inset-y-0 left-0 pl-3.5 flex items-center pointer-events-none text-slate-400">
                                        <i class="fa-brands fa-whatsapp text-lg text-emerald-600"></i>
                                    </div>
                                    <input type="tel" id="phone" name="phone" placeholder="(98) 90000-0000" maxlength="15" required
                                        oninput="maskPhone(this)"
                                        class="w-full pl-10 pr-4 py-3 rounded-xl border border-slate-300 focus:ring-2 focus:ring-brand-500 focus:border-brand-500 text-sm font-semibold bg-slate-50">
                                </div>
                            </div>

                            <!-- SUBMIT BUTTON -->
                            <button type="submit" id="submitBtn" class="w-full py-4 px-6 rounded-xl font-extrabold text-white text-base bg-gradient-to-r from-brand-600 to-brand-500 hover:from-brand-700 hover:to-brand-600 transition shadow-lg hover:shadow-xl transform hover:-translate-y-0.5 flex items-center justify-center gap-2">
                                <span>SOLICITAR PROPOSTA NO WHATSAPP</span>
                                <i class="fa-solid fa-arrow-right"></i>
                            </button>

                            <p class="text-[11px] text-center text-slate-400 pt-1">
                                Sem custo algum. Resposta rápida no WhatsApp.
                            </p>
                        </form>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- VALUE CALCULATOR / SHOWCASE SECTION -->
    <section class="py-16 bg-white border-b border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="text-brand-600 font-extrabold text-xs uppercase tracking-widest bg-brand-50 px-3 py-1 rounded-full">Valores Disponíveis</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Quanto Você Precisa Hoje?</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">Escolha a opção ideal para o seu momento financeiro e simule em poucos segundos.</p>
            </div>

            <!-- CARDS DE VALORES -->
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                
                <!-- CARD 1 MIL -->
                <div class="bg-slate-50 border border-slate-200 rounded-2xl p-6 hover:shadow-xl transition-all duration-300 relative group flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-brand-100 text-brand-700 flex items-center justify-center font-bold text-xl mb-4 group-hover:scale-110 transition">
                            <i class="fa-solid fa-seedling"></i>
                        </div>
                        <span class="text-xs font-bold text-slate-400 uppercase tracking-wider">A partir de</span>
                        <h3 class="text-3xl font-black text-slate-900 my-1">R$ 1.000</h3>
                        <p class="text-slate-500 text-xs mb-4">Ideal para emergências imediatas ou organizar o mês.</p>
                        <ul class="space-y-2 text-xs text-slate-600 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Sem burocracia</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Liberação rápida no PIX</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Parcelas acessíveis</li>
                        </ul>
                    </div>
                    <a href="#simulador" onclick="selectQuickValue('1000')" class="w-full text-center py-2.5 rounded-xl border-2 border-brand-600 text-brand-700 font-bold text-xs hover:bg-brand-600 hover:text-white transition">
                        SIMULAR R$ 1 MIL
                    </a>
                </div>

                <!-- CARD 3 MIL -->
                <div class="bg-slate-50 border border-slate-200 rounded-2xl p-6 hover:shadow-xl transition-all duration-300 relative group flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-emerald-100 text-emerald-700 flex items-center justify-center font-bold text-xl mb-4 group-hover:scale-110 transition">
                            <i class="fa-solid fa-money-bill-trend-up"></i>
                        </div>
                        <span class="text-xs font-bold text-slate-400 uppercase tracking-wider">Mais Procurado</span>
                        <h3 class="text-3xl font-black text-slate-900 my-1">R$ 3.000</h3>
                        <p class="text-slate-500 text-xs mb-4">Excelente para viagens, reformas ou oportunidade de negócio.</p>
                        <ul class="space-y-2 text-xs text-slate-600 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Condições especiais</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Processo 100% digital</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Análise personalizada</li>
                        </ul>
                    </div>
                    <a href="#simulador" onclick="selectQuickValue('3000')" class="w-full text-center py-2.5 rounded-xl border-2 border-brand-600 text-brand-700 font-bold text-xs hover:bg-brand-600 hover:text-white transition">
                        SIMULAR R$ 3 MIL
                    </a>
                </div>

                <!-- CARD 5 MIL -->
                <div class="bg-white border-2 border-brand-500 rounded-2xl p-6 shadow-lg hover:shadow-2xl transition-all duration-300 relative group flex flex-col justify-between">
                    <div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-brand-600 text-white text-[10px] font-black uppercase px-3 py-0.5 rounded-full">
                        Recomendado
                    </div>
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-brand-600 text-white flex items-center justify-center font-bold text-xl mb-4 group-hover:scale-110 transition">
                            <i class="fa-solid fa-vault"></i>
                        </div>
                        <span class="text-xs font-bold text-brand-600 uppercase tracking-wider">Popular</span>
                        <h3 class="text-3xl font-black text-slate-900 my-1">R$ 5.000</h3>
                        <p class="text-slate-500 text-xs mb-4">Perfeito para quitar dívidas ou realizar novos investimentos.</p>
                        <ul class="space-y-2 text-xs text-slate-600 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Prazos de pagamento estendidos</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Taxas competitivas</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Sem taxas antecipadas</li>
                        </ul>
                    </div>
                    <a href="#simulador" onclick="selectQuickValue('5000')" class="w-full text-center py-2.5 rounded-xl bg-brand-600 text-white font-bold text-xs hover:bg-brand-700 transition shadow-md">
                        SIMULAR R$ 5 MIL
                    </a>
                </div>

                <!-- CARD 10 MIL -->
                <div class="bg-slate-50 border border-slate-200 rounded-2xl p-6 hover:shadow-xl transition-all duration-300 relative group flex flex-col justify-between">
                    <div>
                        <div class="w-12 h-12 rounded-xl bg-amber-100 text-amber-700 flex items-center justify-center font-bold text-xl mb-4 group-hover:scale-110 transition">
                            <i class="fa-solid fa-crown"></i>
                        </div>
                        <span class="text-xs font-bold text-slate-400 uppercase tracking-wider">Alto Valor</span>
                        <h3 class="text-3xl font-black text-slate-900 my-1">R$ 10.000+</h3>
                        <p class="text-slate-500 text-xs mb-4">Para grandes planos, conquistas ou reestruturação de finanças.</p>
                        <ul class="space-y-2 text-xs text-slate-600 mb-6">
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Atendimento prioritário VIP</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Melhores prazos</li>
                            <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-600"></i> Análise personalizada de margem</li>
                        </ul>
                    </div>
                    <a href="#simulador" onclick="selectQuickValue('10000')" class="w-full text-center py-2.5 rounded-xl border-2 border-brand-600 text-brand-700 font-bold text-xs hover:bg-brand-600 hover:text-white transition">
                        SIMULAR R$ 10 MIL+
                    </a>
                </div>

            </div>
        </div>
    </section>

    <!-- TARGET AUDIENCE SECTION -->
    <section class="py-16 bg-slate-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="text-brand-600 font-extrabold text-xs uppercase tracking-widest bg-white px-3 py-1 rounded-full shadow-sm">Público Atendido</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Modalidades de Crédito para Seu Perfil</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">Trabalhamos com condições específicas para cada categoria profissional e benefício.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                
                <!-- APOSENTADOS E PENSIONISTAS -->
                <div class="bg-white rounded-2xl p-6 shadow-md border border-slate-200/80 hover:-translate-y-1 transition duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-brand-50 text-brand-600 flex items-center justify-center text-2xl mb-4">
                        <i class="fa-solid fa-person-cane"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Aposentados & Pensionistas</h3>
                    <p class="text-xs text-slate-500 leading-relaxed mb-4">
                        Crédito Consignado INSS com desconto direto no benefício, excelentes prazos e taxas reduzidas.
                    </p>
                    <span class="inline-block text-[11px] font-bold text-brand-700 bg-brand-50 px-2.5 py-1 rounded-md">
                        <i class="fa-solid fa-check text-brand-600 mr-1"></i> Benefício Aprovado
                    </span>
                </div>

                <!-- SERVIDORES PÚBLICOS -->
                <div class="bg-white rounded-2xl p-6 shadow-md border border-slate-200/80 hover:-translate-y-1 transition duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-blue-50 text-blue-600 flex items-center justify-center text-2xl mb-4">
                        <i class="fa-solid fa-building-columns"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Servidores Públicos</h3>
                    <p class="text-xs text-slate-500 leading-relaxed mb-4">
                        Condições exclusivas para Servidores Estaduais e Federais com margem consignável diferenciada.
                    </p>
                    <span class="inline-block text-[11px] font-bold text-blue-700 bg-blue-50 px-2.5 py-1 rounded-md">
                        <i class="fa-solid fa-check text-blue-600 mr-1"></i> Estadual e Federal
                    </span>
                </div>

                <!-- TRABALHADORES CLT -->
                <div class="bg-white rounded-2xl p-6 shadow-md border border-slate-200/80 hover:-translate-y-1 transition duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-emerald-50 text-emerald-600 flex items-center justify-center text-2xl mb-4">
                        <i class="fa-solid fa-user-tie"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Trabalhadores CLT</h3>
                    <p class="text-xs text-slate-500 leading-relaxed mb-4">
                        Antecipação de Saque-Aniversário do FGTS e modalidades de crédito privado para carteira assinada.
                    </p>
                    <span class="inline-block text-[11px] font-bold text-emerald-700 bg-emerald-50 px-2.5 py-1 rounded-md">
                        <i class="fa-solid fa-check text-emerald-600 mr-1"></i> Carteira Assinada
                    </span>
                </div>

                <!-- FORÇAS ARMADAS -->
                <div class="bg-white rounded-2xl p-6 shadow-md border border-slate-200/80 hover:-translate-y-1 transition duration-300">
                    <div class="w-14 h-14 rounded-2xl bg-amber-50 text-amber-700 flex items-center justify-center text-2xl mb-4">
                        <i class="fa-solid fa-shield-halved"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 mb-2">Forças Armadas</h3>
                    <p class="text-xs text-slate-500 leading-relaxed mb-4">
                        Atendimento especializado para militares das Forças Armadas com agilidade na liberação.
                    </p>
                    <span class="inline-block text-[11px] font-bold text-amber-800 bg-amber-50 px-2.5 py-1 rounded-md">
                        <i class="fa-solid fa-check text-amber-600 mr-1"></i> Marinha, Exército e Aeronáutica
                    </span>
                </div>

            </div>
        </div>
    </section>

    <!-- ADVANTAGES SECTION -->
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                
                <div>
                    <span class="text-brand-600 font-extrabold text-xs uppercase tracking-widest bg-brand-50 px-3 py-1 rounded-full">Por Que Escolher a Gente?</span>
                    <h2 class="text-3xl font-black text-slate-900 mt-3 mb-6">Atendimento Rápido, Seguro e Personalizado</h2>
                    
                    <div class="space-y-6">
                        <div class="flex gap-4">
                            <div class="w-10 h-10 rounded-xl bg-brand-100 text-brand-700 flex items-center justify-center shrink-0 font-bold">
                                <i class="fa-solid fa-bolt"></i>
                            </div>
                            <div>
                                <h4 class="text-base font-bold text-slate-900">Pix Na Conta</h4>
                                <p class="text-xs text-slate-500 mt-1">Após aprovação e contratação, o dinheiro é creditado via Pix direto na sua conta bancária.</p>
                            </div>
                        </div>

                        <div class="flex gap-4">
                            <div class="w-10 h-10 rounded-xl bg-brand-100 text-brand-700 flex items-center justify-center shrink-0 font-bold">
                                <i class="fa-brands fa-whatsapp text-lg"></i>
                            </div>
                            <div>
                                <h4 class="text-base font-bold text-slate-900">Atendimento 100% via WhatsApp</h4>
                                <p class="text-xs text-slate-500 mt-1">Tire todas as suas dúvidas e envie seus documentos com comodidade pelo WhatsApp.</p>
                            </div>
                        </div>

                        <div class="flex gap-4">
                            <div class="w-10 h-10 rounded-xl bg-brand-100 text-brand-700 flex items-center justify-center shrink-0 font-bold">
                                <i class="fa-solid fa-shield-cat"></i>
                            </div>
                            <div>
                                <h4 class="text-base font-bold text-slate-900">Sem Cobrança Antecipada</h4>
                                <p class="text-xs text-slate-500 mt-1">Nunca cobramos taxa de cadastro ou antecipação. A simulação é totalmente sem custo.</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- CARDS DE CONFIANÇA -->
                <div class="bg-slate-900 rounded-3xl p-8 text-white relative overflow-hidden shadow-2xl">
                    <div class="absolute -top-10 -right-10 w-40 h-40 bg-brand-500/20 rounded-full blur-2xl"></div>
                    <i class="fa-solid fa-quote-left text-4xl text-brand-500/30 mb-4 block"></i>
                    <p class="text-slate-200 text-sm leading-relaxed mb-6 font-medium">
                        "Preenchi meus dados e fui atendido direto no WhatsApp. Deu tudo certo com minha simulação e recebi as orientações bem claras. Recomendo muito!"
                    </p>
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-full bg-brand-500 flex items-center justify-center font-bold text-white text-sm">
                            JS
                        </div>
                        <div>
                            <p class="text-xs font-bold text-white">João Silva</p>
                            <p class="text-[10px] text-slate-400">Servidor Público Estadual</p>
                        </div>
                    </div>

                    <div class="mt-8 pt-6 border-t border-slate-800 flex items-center justify-between text-xs text-slate-400">
                        <span class="flex items-center gap-1 text-yellow-400 font-bold">
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <i class="fa-solid fa-star"></i>
                            <span class="text-white ml-1">4.9 / 5.0</span>
                        </span>
                        <span>Clientes Atendidos em Todo o Brasil</span>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- HOW IT WORKS STEP BY STEP -->
    <section class="py-16 bg-slate-50 border-t border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="text-brand-600 font-extrabold text-xs uppercase tracking-widest bg-brand-100 px-3 py-1 rounded-full">Passo a Passo</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Como Funciona a Contratação?</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">4 passos simples para dar andamento ao seu crédito.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-4 gap-6 relative">
                
                <div class="bg-white p-6 rounded-2xl border border-slate-200 text-center relative z-10">
                    <div class="w-10 h-10 rounded-full bg-brand-600 text-white font-black text-sm flex items-center justify-center mx-auto mb-4">1</div>
                    <h4 class="text-sm font-bold text-slate-900 mb-1">Preencha o Formulário</h4>
                    <p class="text-xs text-slate-500">Informe seu CPF, perfil e valor desejado.</p>
                </div>

                <div class="bg-white p-6 rounded-2xl border border-slate-200 text-center relative z-10">
                    <div class="w-10 h-10 rounded-full bg-brand-600 text-white font-black text-sm flex items-center justify-center mx-auto mb-4">2</div>
                    <h4 class="text-sm font-bold text-slate-900 mb-1">Redirecionamento</h4>
                    <p class="text-xs text-slate-500">Seus dados são organizados e prontos para envio.</p>
                </div>

                <div class="bg-white p-6 rounded-2xl border border-slate-200 text-center relative z-10">
                    <div class="w-10 h-10 rounded-full bg-brand-600 text-white font-black text-sm flex items-center justify-center mx-auto mb-4">3</div>
                    <h4 class="text-sm font-bold text-slate-900 mb-1">Atendimento WhatsApp</h4>
                    <p class="text-xs text-slate-500">Você conversa diretamente com o consultor no WhatsApp.</p>
                </div>

                <div class="bg-white p-6 rounded-2xl border border-slate-200 text-center relative z-10">
                    <div class="w-10 h-10 rounded-full bg-brand-600 text-white font-black text-sm flex items-center justify-center mx-auto mb-4">4</div>
                    <h4 class="text-sm font-bold text-slate-900 mb-1">Conclusão e Pix</h4>
                    <p class="text-xs text-slate-500">Após formalização, o crédito é liberado na sua conta.</p>
                </div>

            </div>

            <div class="mt-12 text-center">
                <a href="#simulador" class="inline-flex items-center gap-2 bg-brand-600 hover:bg-brand-700 text-white font-extrabold px-8 py-4 rounded-full text-sm sm:text-base shadow-lg hover:shadow-xl transition transform hover:-translate-y-0.5">
                    <i class="fa-solid fa-calculator"></i> SIMULAR MEU CRÉDITO AGORA
                </a>
            </div>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="py-16 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <span class="text-brand-600 font-extrabold text-xs uppercase tracking-widest bg-brand-50 px-3 py-1 rounded-full">Dúvidas Frequentes</span>
                <h2 class="text-3xl font-black text-slate-900 mt-3">Perguntas Frequentes</h2>
            </div>

            <div class="space-y-4">
                
                <div class="border border-slate-200 rounded-xl overflow-hidden">
                    <button type="button" onclick="toggleFAQ(1)" class="w-full text-left p-4 font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center bg-slate-50 hover:bg-slate-100 transition">
                        <span>É cobrada alguma taxa antecipada para simular?</span>
                        <i id="faq-icon-1" class="fa-solid fa-chevron-down text-brand-600 transition-transform"></i>
                    </button>
                    <div id="faq-answer-1" class="hidden p-4 text-xs sm:text-sm text-slate-600 border-t border-slate-200 bg-white">
                        <strong>NUNCA!</strong> A simulação é 100% gratuita. NENHUM correspondente bancário idôneo exige pagamentos de taxas para liberar empréstimo.
                    </div>
                </div>

                <div class="border border-slate-200 rounded-xl overflow-hidden">
                    <button type="button" onclick="toggleFAQ(2)" class="w-full text-left p-4 font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center bg-slate-50 hover:bg-slate-100 transition">
                        <span>Como funciona o atendimento pelo WhatsApp?</span>
                        <i id="faq-icon-2" class="fa-solid fa-chevron-down text-brand-600 transition-transform"></i>
                    </button>
                    <div id="faq-answer-2" class="hidden p-4 text-xs sm:text-sm text-slate-600 border-t border-slate-200 bg-white">
                        Assim que preencher os dados, você é redirecionado para o número <strong>(98) 98453-3013</strong> com sua mensagem já montada contendo seu perfil e valor desejado.
                    </div>
                </div>

                <div class="border border-slate-200 rounded-xl overflow-hidden">
                    <button type="button" onclick="toggleFAQ(3)" class="w-full text-left p-4 font-bold text-sm sm:text-base text-slate-900 flex justify-between items-center bg-slate-50 hover:bg-slate-100 transition">
                        <span>Quais perfis podem solicitar?</span>
                        <i id="faq-icon-3" class="fa-solid fa-chevron-down text-brand-600 transition-transform"></i>
                    </button>
                    <div id="faq-answer-3" class="hidden p-4 text-xs sm:text-sm text-slate-600 border-t border-slate-200 bg-white">
                        Atendemos Aposentados e Pensionistas, Servidores Públicos (Estaduais e Federais), Trabalhadores de Carteira Assinada (CLT) e membros das Forças Armadas.
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-slate-950 text-slate-400 py-12 border-t border-slate-800 text-xs">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 space-y-8">
            <div class="flex flex-col md:flex-row justify-between items-center gap-6 border-b border-slate-800 pb-8">
                <div class="flex items-center gap-3">
                    <div class="w-8 h-8 rounded-lg bg-brand-600 flex items-center justify-center text-white font-extrabold text-base">
                        <i class="fa-solid fa-hand-holding-dollar"></i>
                    </div>
                    <span class="text-lg font-black text-white">CRÉDITO<span class="text-brand-500">FÁCIL</span></span>
                </div>
                <div class="flex flex-wrap justify-center gap-6 font-medium text-slate-300">
                    <a href="#simulador" class="hover:text-brand-500 transition">Simulador</a>
                    <a href="#simulador" class="hover:text-brand-500 transition">Aposentados</a>
                    <a href="#simulador" class="hover:text-brand-500 transition">Servidores</a>
                    <a href="#simulador" class="hover:text-brand-500 transition">CLT</a>
                    <a href="#simulador" class="hover:text-brand-500 transition">Forças Armadas</a>
                </div>
            </div>

            <div class="space-y-3 text-slate-500 leading-relaxed text-[11px] text-justify">
                <p>
                    <strong>Aviso Legal e Transparência:</strong> Somos um correspondente bancário em conformidade com as diretrizes da Resolução nº 3.954 do Banco Central do Brasil. Não cobramos nenhuma taxa antecipada para análise de proposta ou liberação de valor.
                </p>
                <p>
                    <strong>Proteção de Dados (LGPD):</strong> As informações fornecidas neste site são utilizadas exclusivamente para a análise do seu pedido de crédito e atendimento via WhatsApp.
                </p>
            </div>

            <div class="pt-4 flex flex-col sm:flex-row justify-between items-center gap-4 text-slate-500 text-[11px]">
                <p>&copy; CRÉDITOFÁCIL. Todos os direitos reservados.</p>
                <div class="flex items-center gap-4">
                    <span class="flex items-center gap-1"><i class="fa-solid fa-lock text-brand-500"></i> Conexão Segura SSL</span>
                </div>
            </div>
        </div>
    </footer>

    <!-- STICKY MOBILE CTA BAR -->
    <div class="md:hidden fixed bottom-0 left-0 right-0 bg-white/95 backdrop-blur-md border-t border-slate-200 p-3 z-50 shadow-2xl">
        <a href="#simulador" class="w-full py-3.5 px-4 bg-brand-600 hover:bg-brand-700 text-white font-extrabold rounded-xl text-sm flex items-center justify-center gap-2 shadow-lg">
            <i class="fa-solid fa-bolt text-yellow-300"></i>
            SIMULAR NO WHATSAPP (R$ 1k a 10k+)
        </a>
    </div>

    <!-- FLOATING WHATSAPP BUTTON -->
    <a href="https://wa.me/5598984533013?text=Ol%C3%A1!%20Gostaria%20de%20fazer%20uma%20simula%C3%A7%C3%A3o%20de%20cr%C3%A9dito." target="_blank" rel="noopener noreferrer" class="fixed bottom-20 md:bottom-6 right-6 z-50 bg-emerald-500 hover:bg-emerald-600 text-white p-3.5 md:p-4 rounded-full shadow-2xl transition-all transform hover:scale-110 flex items-center justify-center group" title="Falar no WhatsApp">
        <i class="fa-brands fa-whatsapp text-2xl md:text-3xl"></i>
        <span class="max-w-0 overflow-hidden whitespace-nowrap group-hover:max-w-xs transition-all duration-500 ease-in-out text-sm font-bold pl-0 group-hover:pl-2">
            Falar no WhatsApp (98) 98453-3013
        </span>
    </a>

    <!-- SUCCESS MODAL -->
    <div id="successModal" class="fixed inset-0 bg-slate-900/80 backdrop-blur-sm z-50 flex items-center justify-center p-4 hidden">
        <div class="bg-white rounded-3xl max-w-md w-full p-6 text-center shadow-2xl relative border border-slate-100">
            <div class="w-16 h-16 bg-brand-100 text-brand-600 rounded-full flex items-center justify-center mx-auto mb-4 text-3xl font-bold">
                <i class="fa-solid fa-check"></i>
            </div>
            
            <h3 class="text-2xl font-black text-slate-900 mb-2">Simulação Pronta!</h3>
            <p class="text-slate-600 text-xs sm:text-sm mb-6 leading-relaxed">
                Excelente, <strong id="modalClientName" class="text-slate-900"></strong>! Seu pedido de simulação no valor de <strong id="modalClientValue" class="text-brand-600"></strong> para o perfil <strong id="modalClientProfile"></strong> foi gerado.
            </p>

            <div class="bg-slate-50 p-4 rounded-xl border border-slate-200 text-left text-xs mb-6 space-y-2">
                <div class="flex justify-between text-slate-500">
                    <span>Atendimento Directo:</span>
                    <span class="font-bold text-slate-800">(98) 98453-3013</span>
                </div>
                <div class="flex justify-between text-slate-500">
                    <span>Início do Atendimento:</span>
                    <span class="font-bold text-emerald-600"><i class="fa-solid fa-circle-check"></i> Immediato via WhatsApp</span>
                </div>
            </div>

            <a id="whatsappDirectLink" href="#" target="_blank" class="w-full py-4 px-6 bg-emerald-600 hover:bg-emerald-700 text-white font-extrabold rounded-xl text-sm flex items-center justify-center gap-2 shadow-lg transition mb-3">
                <i class="fa-brands fa-whatsapp text-lg"></i>
                ABRIR PROPOSTA NO WHATSAPP
            </a>

            <button type="button" onclick="closeModal()" class="text-xs text-slate-400 hover:text-slate-600 font-semibold underline">
                Fechar esta janela
            </button>
        </div>
    </div>

    <script>
        // PHONE NUMBER CONFIGURATION
        const WHATSAPP_PHONE = "5598984533013";

        // MÁSCARA PARA CPF
        function maskCPF(input) {
            let value = input.value.replace(/\D/g, '');
            if (value.length > 11) value = value.slice(0, 11);

            value = value.replace(/(\d{3})(\d)/, '$1.$2');
            value = value.replace(/(\d{3})(\d)/, '$1.$2');
            value = value.replace(/(\d{3})(\d{1,2})$/, '$1-$2');

            input.value = value;
        }

        // MÁSCARA PARA TELEFONE/WHATSAPP
        function maskPhone(input) {
            let value = input.value.replace(/\D/g, '');
            if (value.length > 11) value = value.slice(0, 11);

            value = value.replace(/^(\d{2})(\d)/g, '($1) $2');
            value = value.replace(/(\d{5})(\d)/, '$1-$2');

            input.value = value;
        }

        // SELEÇÃO DE PERFIL
        function selectProfile(profileName) {
            document.getElementById('selectedProfile').value = profileName;
            document.getElementById('profileError').classList.add('hidden');

            const buttons = document.querySelectorAll('.profile-btn');
            buttons.forEach(btn => {
                if (btn.innerText.includes(profileName)) {
                    btn.classList.add('border-brand-600', 'bg-brand-50', 'text-brand-800');
                    btn.classList.remove('border-slate-200', 'bg-slate-50');
                } else {
                    btn.classList.remove('border-brand-600', 'bg-brand-50', 'text-brand-800');
                    btn.classList.add('border-slate-200', 'bg-slate-50');
                }
            });
        }

        // ATALHO RÁPIDO DE VALORES
        function selectQuickValue(val) {
            const select = document.getElementById('valorDesejado');
            select.value = val;
            
            const chips = document.querySelectorAll('.chip-val');
            chips.forEach(chip => {
                if (chip.innerText.includes(val === '10000' ? '10 MIL+' : val.replace('000', ' MIL'))) {
                    chip.classList.add('bg-brand-600', 'text-white', 'border-brand-600');
                    chip.classList.remove('bg-slate-800/90', 'text-brand-500');
                } else {
                    chip.classList.remove('bg-brand-600', 'text-white', 'border-brand-600');
                    chip.classList.add('bg-slate-800/90', 'text-brand-500');
                }
            });
        }

        // ACCORDION FAQ
        function toggleFAQ(num) {
            const answer = document.getElementById(`faq-answer-${num}`);
            const icon = document.getElementById(`faq-icon-${num}`);
            
            if (answer.classList.contains('hidden')) {
                answer.classList.remove('hidden');
                icon.classList.add('rotate-180');
            } else {
                answer.classList.add('hidden');
                icon.classList.remove('rotate-180');
            }
        }

        // SUBMISSÃO DO FORMULÁRIO COM SIMULAÇÃO PARA O WHATSAPP
        function handleFormSubmit(event) {
            event.preventDefault();

            const profile = document.getElementById('selectedProfile').value;
            const profileError = document.getElementById('profileError');
            
            if (!profile) {
                profileError.classList.remove('hidden');
                return;
            }

            const fullName = document.getElementById('fullName').value;
            const cpf = document.getElementById('cpf').value;
            const phone = document.getElementById('phone').value;
            const valorSelect = document.getElementById('valorDesejado');
            const valorText = valorSelect.options[valorSelect.selectedIndex].text.split('(')[0].trim();

            const submitBtn = document.getElementById('submitBtn');
            submitBtn.disabled = true;
            submitBtn.innerHTML = `<i class="fa-solid fa-spinner animate-spin"></i> Preparando no WhatsApp...`;

            setTimeout(() => {
                submitBtn.disabled = false;
                submitBtn.innerHTML = `<span>SOLICITAR PROPOSTA NO WHATSAPP</span> <i class="fa-solid fa-arrow-right"></i>`;

                // Preencher dados do Modal
                document.getElementById('modalClientName').innerText = fullName;
                document.getElementById('modalClientValue').innerText = `R$ ${valorText}`;
                document.getElementById('modalClientProfile').innerText = profile;

                // Monta mensagem formatada do WhatsApp
                const message = encodeURIComponent(
                    `Olá! Vim do site e gostaria de simular meu crédito/benefício:\n\n` +
                    `👤 *Nome:* ${fullName}\n` +
                    `🪪 *CPF:* ${cpf}\n` +
                    `💼 *Perfil:* ${profile}\n` +
                    `💰 *Valor Pretendido:* R$ ${valorText}\n` +
                    `📱 *Contato:* ${phone}`
                );
                
                const finalUrl = `https://api.whatsapp.com/send?phone=${WHATSAPP_PHONE}&text=${message}`;
                
                document.getElementById('whatsappDirectLink').href = finalUrl;

                // Abre a modal e redireciona automaticamente em seguida
                document.getElementById('successModal').classList.remove('hidden');
                window.open(finalUrl, '_blank');
            }, 800);
        }

        function closeModal() {
            document.getElementById('successModal').classList.add('hidden');
        }
    </script>
</body>
</html>
