    TEAM_TROOPER = DarkRP.createJob("Clone Trooper",{
	color = Color(0, 255, 0, 255),
	model = "models/player/trooper/cctrooper.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "trooper",
	max = 0,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Clones",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "trooper" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CM = DarkRP.createJob("Clone Medic",{
	color = Color(0, 255, 0, 255),
	model = "models/player/testm/cmedic.mdl",
	description = [[You heal clones]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "weapon_medkit"},
	command = "medic",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Medics",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cm" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CMLT = DarkRP.createJob("Clone Medic Lieutenant",{
	color = Color(0, 255, 0, 255),
	model = "models/player/mediclt/cmedic lt.mdl",
	description = [[You heal clones]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "weapon_medkit"},
	command = "mediclt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Medics",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cmlt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CMCO = DarkRP.createJob("Clone Medic Commander",{
	color = Color(0, 255, 0, 255),
	model = "models/player/medicc/cmedic c.mdl",
	description = [[You heal clones]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "weapon_medkit"},
	command = "medicco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Medics",
	PlayerSpawn = function(ply) ply:SetHealth(400) end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cmco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_GG = DarkRP.createJob("General's Guard",{
	color = Color(255, 0, 0, 255),
	model = "models/player/csf/csf.mdl",
	description = [[You guard the General]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "gg",
	max = 3,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	PlayerSpawn = function(ply) ply:SetHealth("300") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "gg" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_GGCO = DarkRP.createJob("General's Guard Commander",{
	color = Color(255, 0, 0, 255),
	model = "models/player/stooge/stooge.mdl",
	description = [[You guard the General]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "ggco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "ggco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT",
})

    TEAM_CADET = DarkRP.createJob("Clone Cadet",{
	color = Color(0, 17, 92, 255),
	model = "models/player/testc/cgi cadet.mdl",
	description = [[You are in training]],
	weapons = {},
	command = "cadet",
	max = 0,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Clones",
})

    TEAM_PILOT = DarkRP.createJob("Clone Pilot",{
	color = Color(0, 255, 0, 255),
	model = "models/player/testctp/clonepilot.mdl",
	description = [[You are to fly fighters and transports]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "pilot",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Clones",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "pilot" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_501ST = DarkRP.createJob("501st Trooper",{
	color = Color(0, 255, 0, 255),
	model = "models/player/501st/c501st.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "501sttrooper",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "501st",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "501st" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_501STSGT = DarkRP.createJob("501st Sergeant",{
	color = Color(0, 255, 0, 255),
	model = "models/player/noble/noble.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "501stsgt",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "501st",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "501st" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_501STLT = DarkRP.createJob("501st Lieutenant",{
	color = Color(0, 255, 0, 255),
	model = "models/player/501stlt/c501stlt.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17dual"},
	command = "501stlt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
    category = "501st",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "501stlt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_501STCO = DarkRP.createJob("501st Commander",{
	color = Color(0, 47, 255, 255),
	model = "models/player/test/rex.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "501stco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "501st",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "501stco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_212TH = DarkRP.createJob("212th Trooper",{
	color = Color(255, 128, 0, 255),
	model = "models/player/212th/c212th trooper.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "212thtrooper",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "212th",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "212th" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_212THSGT = DarkRP.createJob("212th Sergeant",{
	color = Color(255, 128, 0, 255),
	model = "models/player/ender/eender.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "212thsgt",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "212th",
    customCheck = function(ply) return ply:GetNWString("usergroup") == "212thsgt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_212THLT = DarkRP.createJob("212th Lieutenant",{
	color = Color(255, 128, 0, 255),
	model = "models/player/212thlt/c212thlt.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "212thllt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "212th",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "212thlt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_212THCO = DarkRP.createJob("212th Commander",{
	color = Color(0, 47, 255, 255),
	model = "models/player/testccc/ccody.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "212thco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "212th",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "212thco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_WOLFPACK = DarkRP.createJob("104th WolfPack Trooper",{
	color = Color(0, 0, 0, 255),
	model = "models/player/testgr/c104th trooper.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "wolfpack",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Wolfpack",
    customCheck = function(ply) return ply:GetNWString("usergroup") == "104th" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_WOLFPACKP = DarkRP.createJob("104th WolfPack Recon",{
	color = Color(0, 0, 0, 255),
	model = "models/player/104a/104a.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_t700", "weapon_752_dc17"},
	command = "wolfpackr",
	max = 3,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Wolfpack",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "104thp" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_WOLFPACKLT = DarkRP.createJob("104th WolfPack Lieutenant",{
	color = Color(0, 0, 0, 255),
	model = "models/player/104thlt/c104thlt.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "wolfpacklt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Wolfpack",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "104thlt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})
    
    TEAM_WOLFPACKCPT = DarkRP.createJob("104th Wolfpack Captain",{
	color = Color(0, 0, 0, 255),
	model = "models/player/shadow/shadow.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "wolfpackcpt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Wolfpack",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "104thcpt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_WOLFPACK = DarkRP.createJob("104th WolfPack Commander",{
	color = Color(0, 0, 0, 255),
	model = "models/player/wolffe/ccgi wolffe.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "wolfpackco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Wolfpack",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "104thco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_ARC = DarkRP.createJob("Arc Trooper",{
	color = Color(255, 0, 0, 255),
	model = "models/player/barc/cgicbarc.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "arc",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Arc",
	PlayerSpawn = function(ply) ply:SetHealth("200") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "arc" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_ARCSGT = DarkRP.createJob("Arc Drill Sergeant",{
	color = Color(255, 0, 0, 255),
	model = "models/player/shepard/shepard.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "arcSGT",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Arc",
	PlayerSpawn = function(ply) ply:SetHealth("200") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "arcds" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_ARCLT = DarkRP.createJob("Arc Lieutenant",{
	color = Color(255, 0, 0, 255),
	model = "models/player/rarc/cgirarc.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "arclt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Arc",
	PlayerSpawn = function(ply) ply:SetHealth("200") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "arclt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_ARCCO = DarkRP.createJob("Arc Commander",{
	color = Color(255, 0, 0, 255),
	model = "models/player/yarc/cgicyarc.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "arcco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Arc",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "arcco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_41ST = DarkRP.createJob("41st Trooper",{
	color = Color(94, 94, 94, 255),
	model = "models/player/41st/c41st.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "41st",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "41st",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "41st" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_41STLT = DarkRP.createJob("41st Lieutenant",{
	color = Color(94, 94, 94, 255),
	model = "models/player/41stlt/c41stlt.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "41stlt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "41st",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "41stlt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_41STCO = DarkRP.createJob("41st Commander",{
	color = Color(94, 94, 94, 255),
	model = "models/player/testg/cgi gree.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "41stco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "41st",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "41stco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CG = DarkRP.createJob("Clone Guard Trooper",{
	color = Color(138, 0, 0, 255),
	model = "models/player/cguard/cgi cguard.mdl",
	description = [[You guard for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "stunstick"},
	command = "cg",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "CG",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cg" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CGSGT = DarkRP.createJob("Clone Guard Sergeant",{
	color = Color(138, 0, 0, 255),
	model = "models/player/cgco/cgco.mdl",
	description = [[You guard for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "stunstick"},
	command = "cgsgt",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "CG",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cgsgt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CGLT = DarkRP.createJob("Clone Guard lt",{
	color = Color(138, 0, 0, 255),
	model = "models/player/cguardlt/ccguardlt.mdl",
	description = [[You guard for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17", "stunstick", "arrest_stick"},
	command = "cglt",
	max = 3,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "CG",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cglt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CGCPT = DarkRP.createJob("Clone Guard Captain",{
	color = Color(138, 0, 0, 255),
	model = "models/player/kal/cgikal.mdl",
	description = [[You guard for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17", "stunstick", "arrest_stick"},
	command = "cgcpt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "CG",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cgcpt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_CGCO = DarkRP.createJob("Clone Guard Commander",{
	color = Color(138, 0, 0, 255),
	model = "models/player/fox/ccfox.mdl",
	description = [[You guard for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17", "stunstick", "arrest_stick"},
	command = "cgco",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	category = "CG",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "cgco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_327TH = DarkRP.createJob("327th Trooper",{
	color = Color(255, 255, 0, 255),
	model = "models/player/327th/c327tht.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s"},
	command = "327th",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "327th",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "327th" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_327THLT = DarkRP.createJob("327th Lieutenant",{
	color = Color(255, 255, 0, 255),
	model = "models/player/327thlt/c327th lt.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "327thlt",
	max = 2,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "327th",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "327thlt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_327THCO = DarkRP.createJob("327th Commander",{
	color = Color(255, 255, 0, 255),
	model = "models/player/bly/cbly.mdl",
	description = [[You fight for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc17"},
	command = "327thco",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "327th",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "327thco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_38TH = DarkRP.createJob("38th Engineer",{
	color = Color(0, 0, 0, 255),
	model = "models/player/teste/cgi eod.mdl",
	description = [[You Repair for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "repair_tool"},
	command = "38",
	max = 10,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "38th Engineer",
    customCheck = function(ply) return ply:GetNWString("usergroup") == "38th" or ply:IsAdmin() end,
    CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_38THCO = DarkRP.createJob("38th Engineer Commander",{
	color = Color(0, 0, 0, 255),
	model = "models/player/teste/cgi eod.mdl",
	description = [[You Repair for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "repair_tool"},
	command = "38co",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "38th Engineer",
	PlayerSpawn = function(ply) ply:SetHealth("400") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "38thco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_GEN = DarkRP.createJob("General",{
	color = Color(0, 0, 0, 255),
	model = "models/player/arcg/arcg.mdl",
	description = [[You Repair for the Republic]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "repair_tool"},
	command = "gen",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	PlayerSpawn = function(ply) ply:SetHealth("1000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "38thco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_YODA = DarkRP.createJob("Grand Master Yoda",{
	color = Color(0, 255, 0, 255),
	model = "models/player/b4p/b4p_yoda.mdl",
	description = [[Yoda]],
	weapons = {"weapon_lightsaber"},
	command = "yoda",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("10000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "yoda" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_AHSOKA = DarkRP.createJob("Ahsoka",{
	color = Color(0, 255, 0, 255),
	model = "models/jazzmcfly/jka/ashoka/jka_ashoka.mdl",
	description = [[Ahsoka Tano]],
	weapons = {"weapon_lightsaber"},
	command = "AHSOKA",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "ahsoka" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_ANA = DarkRP.createJob("Anakin Skywalker",{
	color = Color(0, 255, 0, 255),
	model = "models/kriegsyntax/sw_752/anakin_est.mdl",
	description = [[Ahsoka Tano]],
	weapons = {"weapon_lightsaber"},
	command = "ana",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("3000") return CLIENT end,
    customCheck = function(ply) return ply:GetNWString("usergroup") == "ana" or ply:IsAdmin() end,
    CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_JEDIP = DarkRP.createJob("Jedi Padawan",{
	color = Color(0, 255, 0, 255),
	model = "models/grealms/characters/padawan/padawan_02.mdl",
	description = [[Jedi]],
	weapons = {"weapon_lightsaber"},
	command = "jedip",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
    customCheck = function(ply) return ply:GetNWString("usergroup") == "padawan" or ply:IsAdmin() end,
    CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_JEDIK = DarkRP.createJob("Jedi Knight",{
	color = Color(0, 255, 0, 255),
	model = "models/grealms/characters/jedirobes/jedirobes_04.mdl",
	description = [[Jedi]],
	weapons = {"weapon_lightsaber"},
	command = "jedik",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("3000") return CLIENT end,
    customCheck = function(ply) return ply:GetNWString("usergroup") == "knight" or ply:IsAdmin() end,
    CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_JEDIM = DarkRP.createJob("Jedi Master",{
	color = Color(0, 255, 0, 255),
	model = "models/grealms/characters/casualjedi/casualjedi_09.mdl",
	description = [[Jedi]],
	weapons = {"weapon_lightsaber"},
	command = "jedim",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("5000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "master" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_ENSIGN = DarkRP.createJob("Ensign",{
	color = Color(0, 0, 0, 255),
	model = "models/player/donut/donut.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "ensign",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "ensign" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_FLT = DarkRP.createJob("Fleet Lieutenant",{
	color = Color(0, 0, 0, 255),
	model = "models/player/donut/donut.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "flt",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "flt" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_LTCO = DarkRP.createJob("Lieutenant Commander",{
	color = Color(0, 0, 0, 255),
	model = "models/player/donut/donut.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "ltco",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "ltco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_FCO = DarkRP.createJob("Fleet Commander",{
	color = Color(0, 0, 0, 255),
	model = "models/lt_c/sci_fi/humans/female_02.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "fco",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "fco" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_FC = DarkRP.createJob("Fleet Captain",{
	color = Color(0, 0, 0, 255),
	model = "models/player/scifi_male_02.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "fc",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "fc" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_RA = DarkRP.createJob("Rear Admiral",{
	color = Color(0, 0, 0, 255),
	model = "models/player/scifi_male_04.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "ra",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "ra" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_VA = DarkRP.createJob("Vice Admiral",{
	color = Color(0, 0, 0, 255),
	model = "models/player/scifi_male_08.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "va",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "va" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_A = DarkRP.createJob("Admiral",{
	color = Color(0, 0, 0, 255),
	model = "models/player/scifi_male_05.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "a",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "admiral" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_FA = DarkRP.createJob("Fleet Admiral",{
	color = Color(0, 0, 0, 255),
	model = "models/player/scifi_male_07.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "fa",
	max = 5,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "fa" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_GA = DarkRP.createJob("Grand Admiral",{
	color = Color(0, 0, 0, 255),
	model = "models/player/scifi_bill.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "ga",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "ga" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_BC = DarkRP.createJob("Battalion Commander",{
	color = Color(245, 255, 0, 255),
	model = "models/player/deviss/ccdeviss.mdl",
	description = [[FLEET]],
	weapons = {"weapon_752_kyd21"},
	command = "bc",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Crew",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "bc" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JOIN THIS REGIMENT"
})

    TEAM_STAFF = DarkRP.createJob("STAFF ON DUTY",{
	color = Color(255, 255, 255, 255),
	model = "models/player/Combine_Super_Soldier.mdl",
	description = [[COOL]],
	weapons = {"weapon_physgun", "gmod_tool", "weapon_752_de10"},
	command = "staff",
	max = 0,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("1000000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "Helper" or ply:IsAdmin() end,
	CustomCheckFailMsg = "STAFF ONLY"
})

    TEAM_BOSS = DarkRP.createJob("RC 1138 Boss",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_38.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "boss",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("3000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "boss" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_SEV = DarkRP.createJob("RC 1207 Sev",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_07.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "sev",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "sev" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"})

    TEAM_FIXER = DarkRP.createJob("RC 1140 Fixer",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_40.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "fixer",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "fixer" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_SCORCH = DarkRP.createJob("RC 1262 Scorch",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_40.mdl",
	description = [[COOL]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn", "weapon_slam", "weapon_swrc_det"},
	command = "scorch",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "scorch" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_NINER = DarkRP.createJob("RC 1309 Niner",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_mp_a.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "niner",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "niner" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_DARMAN = DarkRP.createJob("RC 1136 Darman",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_mp_b.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "darman",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "darman" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_ATIN = DarkRP.createJob("RC 3222 Atin",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_mp_c.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "atin",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "atin" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_CORR = DarkRP.createJob("RC 5108 Corr",{
	color = Color(255, 255, 255, 255),
	model = "models/player/sgg/starwars/clone_commando_mp_d.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "corr",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "corr" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_GREGOR = DarkRP.createJob("CC 5576-39 Gregor",{
	color = Color(255, 255, 255, 255),
	model = "models/player/star wars/gregor/clone_commando_gregor.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc17m_br", "weapon_752_dc15sa", "weapon_752_dc17m_sn"},
	command = "gregor",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("2000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "gregor" or ply:IsAdmin() end,
	CustomCheckFailMsg = "RC only"
})

    TEAM_FIVES = DarkRP.createJob("Fives",{
	color = Color(0, 255, 0, 255),
	model = "models/player/fives/fives.mdl",
	description = [[RC]],
	weapons = {"weapon_752_dc15a", "weapon_752_dc15s", "weapon_752_dc17dual"},
	command = "fives",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	PlayerSpawn = function(ply) ply:SetHealth("300") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "fives" or ply:IsAdmin() end,
	CustomCheckFailMsg = "fives"
})

    TEAM_KENOBI = DarkRP.createJob("Obi Wan Kenobi",{
	color = Color(0, 255, 0, 255),
	model = "models/player/b4p/b4p_obiwan/obiwan.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "obiwan",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "obiwan" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_AAYLA = DarkRP.createJob("Aayla Secura",{
	color = Color(0, 255, 0, 255),
	model = "models/player/nav/aayla.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "aayla",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "aayla" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_KITFISTO = DarkRP.createJob("Kit Fisto",{
	color = Color(0, 255, 0, 255),
	model = "models/player/nav/kitfisto.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "kitfisto",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "kitfisto" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_MUNDI = DarkRP.createJob("Ki adi mundi",{
	color = Color(0, 255, 0, 255),
	model = "models/player/nav/kitfisto.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "kiadimindi",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "mundi" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_PLO = DarkRP.createJob("Plo Koon",{
	color = Color(0, 255, 0, 255),
	model = "models/kriegsyntax/sw_752/plokoon_est.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "plo",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "plokoon" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_MACEWINDU = DarkRP.createJob("Mace Windu",{
	color = Color(0, 255, 0, 255),
	model = "models/ryan7259/mace_windu/mace_windu_player.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "mace",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "macewindu" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_SHAAKTI = DarkRP.createJob("Shaakti",{
	color = Color(0, 255, 0, 255),
	model = "models/ryan7259/shaak_ti_felucia/shaak_ti.mdl",
	description = [[jedi]],
	weapons = {"weapon_lightsaber"},
	command = "shaakti",
	max = 1,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Jedi",
	PlayerSpawn = function(ply) ply:SetHealth("8000") return CLIENT end,
	customCheck = function(ply) return ply:GetNWString("usergroup") == "shaakti" or ply:IsAdmin() end,
	CustomCheckFailMsg = "JEDI"
})

    TEAM_DROID = DarkRP.createJob("Battle Droid",{
	color = Color(0, 255, 0, 255),
	model = "models/player/sgg/starwars/battledroid.mdl",
	description = [[BD]],
	weapons = {"weapon_752_e5"},
	command = "bd",
	max = 0,
	salary = 0,
	admin = 0,
	vote = false,
	hasLicense = false,
	category = "Other",
	customCheck = function(ply) return ply:GetNWString("usergroup") == "superadmin" or ply:IsAdmin() end,
	CustomCheckFailMsg = "bd"
})
