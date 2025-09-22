-- Script pra mostrar compra de gamepass no Roblox
local MarketplaceService = game:GetService("MarketplaceService")
local Players = game:GetService("Players")
local player = Players.LocalPlayer
local gamePassID = 1481989146 -- Troca pelo ID do teu gamepass

-- Função pra abrir a tela de compra
local function promptGamePassPurchase()
    MarketplaceService:PromptGamePassPurchase(player, gamePassID)
end

-- Executa a função assim que o script roda
promptGamePassPurchase()
