// * JOBS.TXT * //
"team"						"2 or 3"		2 - T; 3 - CT;
"name"						"translation job/rank"			[Dont use in unemployed job]
"respawn_time"				"10"			// respawn timer if you dead. 1 or ...
"model"						"model/skin/player.mdl"					// skin/model player
"salary"					"100"
"health"					"150"
"armor"						"150"
"tools"						{ "tool" "weapon_name"  "tool" "weapon_name"  "tool" "weapon_name" }
"tools"						{}		// Do not give weapons
"rookie"					"name rank"			// This is level on the job			[Newbie]
"boss"						"name rank"			// This is level on the job			[Main]
"steal"						"1"					1 - ON; 0 - OFF 		// Steal money, press use [E]
"pvp_amount"				"20"			// If player kill plus for pvp status
"taser"						"1"				1 - ON; 0 - OFF				// Taser [sm_taser]
"arrest"					"1"				1 - ON; 0 - OFF				// Allows to arrest the player
"pvp_enabled"				"0"				1 - ON; 0 - OFF				// Allows the disable pvp
"cuff"						"1"				1 - ON; 0 - OFF				// Allows to put cuffs on the criminal


// * EXAMPLE JOB * //
	"Mafia"			// Job
	{
		"rookie"	"Test"
		"Test"
		{
			"respawn_time" "5"
			"salary" "1"				// salary get money
			"tools" { "tool" "weapon_knife"  "tool" "weapon_deagle" }
			"team" "3"
		}
		
		"Soldier"
		{
			"respawn_time" "5"
			"salary" "4"				// salary get money
			"tools" {}
			"team" "3"
			"steal" "1"			// Steal money - ON
		}
		
		"boss"		"C.Boss"
		"C.Boss"
		{
			"respawn_time" "4"
			"salary" "5"				// salary get money
			"tools" { "tool" "weapon_knife"  "tool" "weapon_awp"}
			"team" "3"
			"steal" "1"			// Steal money - ON
		}
	}