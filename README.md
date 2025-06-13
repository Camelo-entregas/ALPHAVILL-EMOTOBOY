# ALPHAVILL-EMOTOBOY<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ALPHAVILLE MOTOBOY - Entregas Rápidas em Alphaville e Região</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* [Seu CSS existente permanece igual] */
        
        /* Seção do Mapa Aprimorada */
        .coverage {
            padding: 80px 0;
            background-color: var(--white);
            position: relative;
        }
        
        .map-container {
            height: 500px;
            width: 100%;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            margin-top: 40px;
            position: relative;
        }
        
        .map-overlay {
            position: absolute;
            top: 20px;
            left: 20px;
            background: rgba(255, 255, 255, 0.9);
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            z-index: 1000;
            max-width: 300px;
        }
        
        .map-overlay h3 {
            color: var(--primary);
            margin-bottom: 10px;
            font-size: 18px;
        }
        
        .coverage-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 40px;
            background: var(--light);
            padding: 30px;
            border-radius: 10px;
        }
        
        .coverage-list li {
            display: flex;
            align-items: center;
            gap: 10px;
            color: var(--dark);
            padding: 8px 0;
            border-bottom: 1px solid #eee;
        }
        
        .coverage-list i {
            color: var(--secondary);
            font-size: 18px;
        }
        
        .check-coverage {
            background: var(--primary);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 50px;
            font-weight: 600;
            cursor: pointer;
            display: block;
            margin: 30px auto 0;
            transition: all 0.3s;
        }
        
        .check-coverage:hover {
            background: var(--secondary);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
    </style>
</head>
<body>
    <!-- [Seu conteúdo existente permanece igual até a seção About] -->

    <!-- Seção de Cobertura Aprimorada -->
    <section class="coverage">
        <div class="container">
            <h2 class="section-title">Área de Cobertura Exclusiva</h2>
            <p style="text-align: center; margin-bottom: 20px; max-width: 800px; margin-left: auto; margin-right: auto;">
                Nossa equipe atende toda a região de Alphaville e adjacências com rapidez e segurança. 
                Confira no mapa abaixo nossa área de atuação:
            </p>
            
            <div class="map-container">
                <div class="map-overlay">
                    <h3><i class="fas fa-map-marked-alt"></i> Centro de Operações</h3>
                    <p>Alphaville Commercial - Barueri/SP</p>
                </div>
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14639.09632494315!2d-46.857222!3d-23.493333!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94cf03c20ecb7937%3A0x31502f6b8d3c2e15!2sAlphaville%2C%20Barueri%20-%20SP!5e0!3m2!1spt-BR!2sbr!4v1717123456789!5m2!1spt-BR!2sbr" 
                        width="100%" 
                        height="100%" 
                        style="border:0;" 
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
            
            <div class="coverage-list">
                <h3 style="grid-column: 1 / -1; color: var(--primary); margin-bottom: 15px;">
                    <i class="fas fa-check-circle"></i> Bairros Atendidos:
                </h3>
                <li><i class="fas fa-map-pin"></i> Alphaville Industrial</li>
                <li><i class="fas fa-map-pin"></i> Alphaville Comercial</li>
                <li><i class="fas fa-map-pin"></i> Tamboré</li>
                <li><i class="fas fa-map-pin"></i> Jardim Califórnia</li>
                <li><i class="fas fa-map-pin"></i> Aldeia da Serra</li>
                <li><i class="fas fa-map-pin"></i> Vila São Francisco</li>
                <li><i class="fas fa-map-pin"></i> Centro Barueri</li>
                <li><i class="fas fa-map-pin"></i> Jardim Barueri</li>
                <li><i class="fas fa-map-pin"></i> Parque Viana</li>
                <li><i class="fas fa-map-pin"></i> City Boa Vista</li>
            </div>
            
            <button class="check-coverage">
                <i class="fas fa-search-location"></i> Verifique se atendemos seu endereço
            </button>
        </div>
    </section>

    <script>
        // Função para o botão de verificação de cobertura
        document.querySelector('.check-coverage').addEventListener('click', function() {
            const address = prompt("Digite seu endereço completo (Rua, Número, Bairro):");
            if (address) {
                alert("Obrigado! Verificaremos e entraremos em contato para confirmar se atendemos em:\n\n" + address);
            }
        });
    </script>
</body>
</html>
