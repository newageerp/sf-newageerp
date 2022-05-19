# ENV

## auth 
AUTH_KEY=

## base-entity 
AUTH_KEY=

## controlpanel 
FRONT_URL=
NAE_SFS_CP_DB_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_DB_PATH=
NAE_SFS_CP_DB_PATH=
NAE_SFFILES_STORAGE_PUBLIC_DIR=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_DB_PATH=

## export 
NAE_SFS_PUBLIC_DOC_DIR=

## files 
NAE_SFFILES_STORAGE_DIR=
NAE_SFFILES_STORAGE_PUBLIC_DIR=
FRONT_URL=
FRONT_URL=

## mail-smtp 
SF_MAIL_SMTP_HOST=
SF_MAIL_SMTP_USER=
SF_MAIL_SMTP_PSW=
SF_MAIL_SMTP_SECURE=
SF_MAIL_SMTP_PORT=
SF_MAIL_SMTP_FROM_EMAIL=
SF_MAIL_SMTP_FROM_NAME=

## mailjet 
NAE_SFS_MAILJET_PUBLIC_KEY=
NAE_SFS_MAILJET_PRIVATE_KEY=
NAE_SFS_MAILJET_PUBLIC_KEY=

## mails 
APP_ENV=
SF_MAIL_DEV_TEST_EMAIL=

## pdf 
NAE_SFS_TOKEN=
NAE_SFS_FRONT_URL=

## push-messages 
NAE_SFPUSHMESSAGE_FIREBASE_KEY=

## uservice 
NAE_SFS_PROPERTIES_FILE_PATH=
NAE_SFS_SCHEMAS_FILE_PATH=
NAE_SFS_PROPERTIES_FILE_PATH=
NAE_SFS_SCHEMAS_FILE_PATH=


# CONTROLLERS
config/routes/annotations.yaml
sf_auth:
    resource: '@NewageerpSfAuthBundle/Controller'
    type:     annotation
sf_controlpanel:
    resource: '@NewageerpSfControlpanelBundle/Controller'
    type:     annotation
sf_export:
    resource: '@NewageerpSfExportBundle/Controller'
    type:     annotation
sf_files:
    resource: '@NewageerpSfFilesBundle/Controller'
    type:     annotation
sf_import:
    resource: '@NewageerpSfImportBundle/Controller'
    type:     annotation
sf_mails:
    resource: '@NewageerpSfMailBundle/Controller'
    type:     annotation
sf_notes:
    resource: '@NewageerpSfNotesBundle/Controller'
    type:     annotation
sf_pdf:
    resource: '@NewageerpSfPdfBundle/Controller'
    type:     annotation
sf_uservice:
    resource: '@NewageerpSfUserviceBundle/Controller'
    type:     annotation
sf_xlsx:
    resource: '@NewageerpSfXlsxBundle/Controller'
    type:     annotation

# MESSAGE HANDLERS
config/services.yaml
    Newageerp\SfNotes\Messenger\NotesReadAllMessageHandler:
        tags: [messenger.message_handler]