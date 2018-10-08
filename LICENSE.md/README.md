# XLSX-Excel-Code
#Excel XML code for UI5 Fiori application*/

<core:FragmentDefinition xmlns="sap.m" xmlns:u="sap.ui.unified" xmlns:core="sap.ui.core">
	<Dialog title='Upload Excel' contentWidth='1rem'>
		<content>
			<u:FileUploader id="fileUploader" typeMissmatch="handleTypeMissmatchExcel" uploadComplete="handleExcelUploadPress" name="myFileUpload"
					change="handleExcelUploadPress" width="100%" style="Emphasized" placeholder='Upload File' fileType="xlsx"/>
		</content>
		<beginButton>
			<Button text="Clear Text" press="onClearExcelUpload"/>
		</beginButton>
		<endButton>
			<Button text="Close" press="onUploadDialogClose"/>
		</endButton>
	</Dialog>
</core:FragmentDefinition>
