# Info

Name: Infinity RPG NPC Cards

Author: Thomas Young (https://github.com/DrakeRichards)

Date last updated: December 11, 2018


This is a CardMaker (https://github.com/nhmkdev/cardmaker) project. You will need at least version 1.0.0.1 to open it.

## Parts

*	"**Infinity RPG NPC Cards.cmp**"- The project file itself.
*	"**N_Black.png**"- The icon for Combat Dice.
*	"**NPC Stats.csv**"- The data source for this project file. This CSV can be somewhat cumbersome to use, but it is formatted to make rapid entry easy. 
* "**NPC Stats_defines.csv**"- The project's defines file. This is used to insert the Combat Dice icon into the text of the cards.

## Instructions

Most of the work should be done in the data file. Each row in it represents a new card. The columns are organized as such:

* **Copies**: Lists how many copies of the card to make. This should be 1.
* **Name**: The name of the NPC.
* **Classification**: The classification (Trooper/Elite/Nemesis) of the NPC.
* **AGI through WIL**: The attributes of the NPC. Each column MUST have an entry, even if it is 0.
* **Combat EXP through Technical FOC**: The Fields of Expertise for the NPC. These should be simple numbers with no + symbols. If the NPC has a rating of 0 in that field, leave the field blank.
* **Firewall through Armour**: The defenses for the NPC. If the NPC has a rating of 0 in these, leave the field blank.
* **Attacks**: These cards can list 4 attacks, each with up to 2 alternate firing modes. The Attack columns are further organized as such:
  *	**Name**- The name of the attack.
  * **Range/Damage**- The range and damage of the attack. If this field has an entry it will be followed by "N damage, ". You should format this field with the range listed first followed by the damage, and having no trailing spaces.
  * **Qualities**- The Qualities of the attack. This should be a long text field, so input all Qualities of the weapon here.
  *	**Secondary/Tertiary Modes**- These fields follow the conventions of the regular Attacks. If there is no entry in Damage or Qualities, those fields will be left out.
*	**Gear**: The gear of the NPC listed in plain text. Make sure to remove any line breaks if you copy this from the PDF.
*	**Common Special Abilities**: The common abilities of the NPC. List all abilities in the same field, one after the other.
*	**Special Abilities**: The name and descriptive text for up to 4 special abilities.

Once you have inputted the stats for all NPCs that you would like printed, save the data file. Make sure that you keep it as a comma-delimited CSV file. When you open the project in CardMaker, it will be VERY slow to load since there are a lot of conditional formatting tricks going on. You can export and print the cards from the file menu, either as JPGs (for use in roll20 or digital reference) or as PDFs (for printing).
