<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MΩME - Olympiades Mathématiques pour Collégiens</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .custom-bg {
            background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%);
        }
        .logo {
            font-family: 'Times New Roman', serif;
            font-size: 2.5rem;
            font-weight: bold;
        }
        .nav-link:hover {
            transform: translateY(-2px);
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .form-input:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.5);
        }
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        .floating {
            animation: float 3s ease-in-out infinite;
        }
    </style>
</head>
<body class="bg-gray-50 font-sans">
    <!-- Navigation -->
    <nav class="custom-bg text-white shadow-lg">
        <div class="container mx-auto px-6 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-4">
                <span class="logo text-white">MΩME</span>
                <span class="text-xl hidden md:block">Mathématiques Olympique pour les Minis Étudiants</span>
            </div>
            <div class="hidden md:flex items-center space-x-8">
                <a href="#home" class="nav-link px-3 py-2 rounded-md text-sm font-medium bg-blue-700 text-white transition duration-300">Accueil</a>
                <a href="#inscription" class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:bg-blue-700 text-white transition duration-300">Inscription Compétition</a>
                <a href="#membre" class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:bg-blue-700 text-white transition duration-300">Devenir Membre</a>
                <a href="#ressources" class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:bg-blue-700 text-white transition duration-300">Ressources</a>
                <a href="#contact" class="nav-link px-3 py-2 rounded-md text-sm font-medium hover:bg-blue-700 text-white transition duration-300">Contact</a>
            </div>
            <div class="md:hidden">
                <button id="mobile-menu-button" class="text-white focus:outline-none">
                    <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden pb-4 px-6">
            <div class="flex flex-col space-y-2">
                <a href="#home" class="px-3 py-2 rounded-md text-sm font-medium bg-blue-700 text-white">Accueil</a>
                <a href="#inscription" class="px-3 py-2 rounded-md text-sm font-medium text-white hover:bg-blue-700">Inscription Compétition</a>
                <a href="#membre" class="px-3 py-2 rounded-md text-sm font-medium text-white hover:bg-blue-700">Devenir Membre</a>
                <a href="#ressources" class="px-3 py-2 rounded-md text-sm font-medium text-white hover:bg-blue-700">Ressources</a>
                <a href="#contact" class="px-3 py-2 rounded-md text-sm font-medium text-white hover:bg-blue-700">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Page Content -->
    <div id="page-content">
        <!-- Home Page -->
        <div id="home" class="page active">
            <!-- Hero Section -->
            <section class="custom-bg text-white py-20">
                <div class="container mx-auto px-6 flex flex-col md:flex-row items-center">
                    <div class="md:w-1/2 mb-10 md:mb-0">
                        <h1 class="text-4xl md:text-6xl font-bold mb-6">Défiez vos limites en mathématiques !</h1>
                        <p class="text-xl mb-8">Rejoignez les Olympiades MΩME et découvrez le plaisir de résoudre des problèmes mathématiques stimulants.</p>
                        <div class="flex space-x-4">
                            <a href="#inscription" class="bg-white text-blue-800 px-6 py-3 rounded-lg font-bold hover:bg-gray-100 transition duration-300">S'inscrire aux compétitions</a>
                            <a href="#membre" class="border-2 border-white text-white px-6 py-3 rounded-lg font-bold hover:bg-white hover:text-blue-800 transition duration-300">Devenir membre</a>
                        </div>
                    </div>
                    <div class="md:w-1/2 flex justify-center">
                        <div class="relative w-64 h-64 md:w-80 md:h-80 bg-white rounded-full flex items-center justify-center shadow-2xl floating">
                            <span class="text-blue-800 text-9xl font-bold">α</span>
                        </div>
                    </div>
                </div>
            </section>

            <!-- About Section -->
            <section class="py-20 bg-white">
                <div class="container mx-auto px-6">
                    <h2 class="text-4xl font-bold text-center text-gray-800 mb-16">À propos de MΩME</h2>
                    <div class="flex flex-col md:flex-row md:space-x-8">
                        <div class="md:w-1/3 mb-8 md:mb-0">
                            <div class="bg-blue-100 rounded-lg p-6 h-full card-hover transition duration-300">
                                <div class="text-blue-800 mb-4">
                                    <i class="fas fa-bullseye text-4xl"></i>
                                </div>
                                <h3 class="text-2xl font-bold mb-4 text-gray-800">Notre Mission</h3>
                                <p class="text-gray-600">Promouvoir l'excellence en mathématiques chez les collégiens à travers des compétitions stimulantes et un esprit de camaraderie.</p>
                            </div>
                        </div>
                        <div class="md:w-1/3 mb-8 md:mb-0">
                            <div class="bg-blue-100 rounded-lg p-6 h-full card-hover transition duration-300">
                                <div class="text-blue-800 mb-4">
                                    <i class="fas fa-trophy text-4xl"></i>
                                </div>
                                <h3 class="text-2xl font-bold mb-4 text-gray-800">Nos Compétitions</h3>
                                <p class="text-gray-600">Des épreuves adaptées à tous les niveaux, avec des problèmes originaux conçus par notre équipe d'experts en pédagogie mathématique.</p>
                            </div>
                        </div>
                        <div class="md:w-1/3">
                            <div class="bg-blue-100 rounded-lg p-6 h-full card-hover transition duration-300">
                                <div class="text-blue-800 mb-4">
                                    <i class="fas fa-users text-4xl"></i>
                                </div>
                                <h3 class="text-2xl font-bold mb-4 text-gray-800">Notre Communauté</h3>
                                <p class="text-gray-600">Plus de 5 000 collégiens participants chaque année, venant de toute la France pour partager leur passion des mathématiques.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Testimonials -->
            <section class="py-20 bg-gray-100">
                <div class="container mx-auto px-6">
                    <h2 class="text-4xl font-bold text-center text-gray-800 mb-16">Témoignages</h2>
                    <div class="flex flex-col md:flex-row md:space-x-8">
                        <div class="md:w-1/2 mb-8 md:mb-0">
                            <div class="bg-white rounded-lg p-8 shadow-lg card-hover transition duration-300">
                                <div class="flex items-center mb-4">
                                    <div class="text-yellow-400 mr-2">
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                    </div>
                                </div>
                                <p class="text-gray-600 mb-6">"Participant aux Olympiades MΩME depuis deux ans, j'ai énormément progressé en mathématiques et découvert une nouvelle façon de penser. Les problèmes sont passionnants !"</p>
                                <div class="flex items-center">
                                    <div class="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mr-4">
                                        <span class="text-blue-800 font-bold">L</span>
                                    </div>
                                    <div>
                                        <h4 class="font-bold text-gray-800">Léa, 14 ans</h4>
                                        <p class="text-gray-500">Collège Les Cèdres, Lyon</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="md:w-1/2">
                            <div class="bg-white rounded-lg p-8 shadow-lg card-hover transition duration-300">
                                <div class="flex items-center mb-4">
                                    <div class="text-yellow-400 mr-2">
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                        <i class="fas fa-star"></i>
                                    </div>
                                </div>
                                <p class="text-gray-600 mb-6">"En tant que professeur, je recommande vivement MΩME à mes élèves. L'approche ludique et stimulante des mathématiques est un complément parfait au programme scolaire."</p>
                                <div class="flex items-center">
                                    <div class="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mr-4">
                                        <span class="text-blue-800 font-bold">P</span>
                                    </div>
                                    <div>
                                        <h4 class="font-bold text-gray-800">Prof. Martin</h4>
                                        <p class="text-gray-500">Collège Jean Moulin, Paris</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </div>

        <!-- Inscription Compétition Page -->
        <div id="inscription" class="page hidden">
            <section class="py-20 bg-white">
                <div class="container mx-auto px-6 max-w-4xl">
                    <h2 class="text-4xl font-bold text-center text-gray-800 mb-12">Inscription aux Compétitions MΩME</h2>
                    
                    <div class="bg-blue-50 rounded-lg p-8 shadow-lg">
                        <form id="competition-form" class="space-y-6">
                            <div>
                                <h3 class="text-xl font-semibold text-gray-800 mb-4">Informations Personnelles</h3>
                                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                    <div>
                                        <label for="first-name" class="block text-sm font-medium text-gray-700 mb-1">Prénom</label>
                                        <input type="text" id="first-name" name="first-name" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500" required>
                                    </div>
                                    <div>
                                        <label for="last-name" class="block text-sm font-medium text-gray-700 mb-1">Nom</label>
                                        <input type="text" id="last-name" name="last-name" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500" required>
                                    </div>
                                    <div>
                                        <label for="birthdate" class="block text-sm font-medium text-gray-700 mb-1">Date de Naissance</label>
                                        <input type="date" id="birthdate" name="birthdate" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500" required>
                                    </div>
                                    <div>
                                        <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                                        <input type="email" id="email" name="email" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500" required>
                                    </div>
                                </div>
                            </div>

                            <div>
                                <h3 class="text-xl font-semibold text-gray-800 mb-4">Informations Scolaires</h3>
                                <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                                    <div>
                                        <label for="school" class="block text-sm font-medium text-gray-700 mb-1">Établissement Scolaire</label>
                                        <input type="text" id="school" name="school" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500" required>
                                    </div>
                                    <div>
                                        <label for="class" class="block text-sm font-medium text-gray-700 mb-1">Classe</label>
                                        <select id="class" name="class" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500" required>
                                            <option value="">Sélectionnez votre classe</option>
                                            <option value="6eme">6ème</option>
                                            <option value="5eme">5ème</option>
                                            <option value="4eme">4ème</option>
                                            <option value="3eme">3ème</option>
                                        </select>
                                    </div>
                                </div>
                            </div>

                            <div>
                                <h3 class="text-xl font-semibold text-gray-800 mb-4">Compétition</h3>
                                <div class="space-y-4">
                                    <div class="flex items-center">
                                        <input type="radio" id="individual" name="competition-type" value="individual" class="h-4 w-4 text-blue-600 focus:ring-blue-500" checked>
                                        <label for="individual" class="ml-3 block text-sm font-medium text-gray-700">Individuelle</label>
                                    </div>
                                    <div class="flex items-center">
                                        <input type="radio" id="team" name="competition-type" value="team" class="h-4 w-4 text-blue-600 focus:ring-blue-500">
                                        <label for="team" class="ml-3 block text-sm font-medium text-gray-700">Par équipe (3-4 élèves du même établissement)</label>
                                    </div>
                                </div>
                            </div>

                            <div id="team-members" class="hidden">
                                <h3 class="text-xl font-semibold text-gray-800 mb-4">Membres de l'Équipe</h3>
                                <div class="space-y-4">
                                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                        <div>
                                            <label for="member1-name" class="block text-sm font-medium text-gray-700 mb-1">Nom et Prénom Membre 1</label>
                                            <input type="text" id="member1-name" name="member1-name" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500">
                                        </div>
                                        <div>
                                            <label for="member1-email" class="block text-sm font-medium text-gray-700 mb-1">Email Membre 1</label>
                                            <input type="email" id="member1-email" name="member1-email" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500">
                                        </div>
                                    </div>
                                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                        <div>
                                            <label for="member2-name" class="block text-sm font-medium text-gray-700 mb-1">Nom et Prénom Membre 2</label>
                                            <input type="text" id="member2-name" name="member2-name" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500">
                                        </div>
                                        <div>
                                            <label for="member2-email" class="block text-sm font-medium text-gray-700 mb-1">Email Membre 2</label>
                                            <input type="email" id="member2-email" name="member2-email" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500">
                                        </div>
                                    </div>
                                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                        <div>
                                            <label for="member3-name" class="block text-sm font-medium text-gray-700 mb-1">Nom et Prénom Membre 3</label>
                                            <input type="text" id="member3-name" name="member3-name" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500">
                                        </div>
                                        <div>
                                            <label for="member3-email" class="block text-sm font-medium text-gray-700 mb-1">Email Membre 3</label>
                                            <input type="email" id="member3-email" name="member3-email" class="form-input w-full px-4 py-2 rounded-lg border border-gray-300 focus:border-blue-500">
                                        </div>
       
