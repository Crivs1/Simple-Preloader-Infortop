# Simple Preloader Infortop

Preloader simples e leve para WordPress. Mostra uma imagem (logo/SVG/PNG/GIF) com fade curto, **sem bloquear o render**.

## ✨ Funcionalidades
- Escolher **imagem** pelo Media Library
- **Background** configurável (cor + opacidade)
- **Largura** da imagem (px)
- **Duração mínima** + **fade out**
- **Só 1.ª visita** (usa `localStorage`)
- **Apenas na homepage**
- **Ignorar utilizadores autenticados**
- **ON/OFF** rápido
- **Preview forçado**: adicionar `?spi_preview=1` ao URL

## Requisitos
- WordPress 5.8+
- PHP 7.4+

## Instalação
1. Download do ficheiro `.zip` (em Releases) **ou** cria tu:
   - Comprime a pasta `simple-preloader-infortop` com este conteúdo.
2. WP Admin → **Plugins → Adicionar novo → Enviar plugin**.
3. Ativar.
4. Configurar em **Definições → Simple Preloader**.

## Sugestões de configuração
- **Imagem**: logo SVG/PNG ≤ 20 KB  
- **Background**: `#000000` com opacidade **0.00** (transparente) ou ~0.35 (escurecido)  
- **Largura**: 110 px  
- **Duração mínima**: 900–1500 ms  
- **Fade out**: 250–300 ms  
- **Só 1.ª visita**: ligado  
- **Apenas homepage**: ligado  
- **Ignorar autenticado**: ligado

## FAQ
**O tempo mínimo não está a ser respeitado?**  
Desde a v1.2.0 é **sempre** respeitado. Se tiveres “Fechar ao terminar de carregar” ligado, o fecho acontece **após** cumprir o mínimo.

**Quero testar mesmo com “Só 1.ª visita”.**  
Usa `?spi_preview=1` numa página e o preloader aparece.

## Desenvolvimento
- Branch principal: `main`
- Versões seguem SemVer (ex.: `1.2.1`)
- Ao criares um tag (`v1.2.1`), o GitHub Action gera um **ZIP** na página de Releases.

## Licença
MIT — ver `LICENSE`.
