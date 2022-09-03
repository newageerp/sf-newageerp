# ENV

## auth 
AUTH_KEY=
NAE_SFS_MAILJET_DEFAULT_SENDER=
NAE_SFS_FRONT_URL=

## base-entity 
AUTH_KEY=

## controlpanel 
FRONT_URL=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_CP_DB_PATH=
NAE_SFS_CP_DB_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_FRONT_URL=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_ROOT_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_STORAGE_PATH=
NAE_SFS_CP_DB_PATH=

## event-listener 
NAE_SFS_RBQ_HOST=
NAE_SFS_RBQ_PORT=
NAE_SFS_RBQ_USER=
NAE_SFS_RBQ_PASSWORD=
FRONT_REMOTE_URL=

## export 
NAE_SFS_PUBLIC_DOC_DIR=

## files 
NAE_SFFILES_STORAGE_DIR=
NAE_SFFILES_STORAGE_PUBLIC_DIR=
FRONT_URL=
FRONT_URL=
NAE_SFS_FRONT_URL=

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
NAE_SFS_TOKEN=
NAE_SFS_FRONT_URL=

## push-messages 
NAE_SFPUSHMESSAGE_FIREBASE_KEY=

## socket 
WS_REDIS_DSN=
NAE_SFS_RBQ_HOST=
NAE_SFS_RBQ_PORT=
NAE_SFS_RBQ_USER=
NAE_SFS_RBQ_PASSWORD=
NAE_SFS_RBQ_QUEUE=

## uservice 
NAE_SFS_PROPERTIES_FILE_PATH=
NAE_SFS_SCHEMAS_FILE_PATH=
NAE_SFS_PROPERTIES_FILE_PATH=
NAE_SFS_SCHEMAS_FILE_PATH=
NAE_SFS_CP_STORAGE_PATH=


# CONTROLLERS
config/routes/annotations.yaml
sf_auth:
    resource: '@NewageerpSfAuthBundle/Controller'
    type:     annotation
sf_bookmarks:
    resource: '@NewageerpSfBookmarksBundle/Controller'
    type:     annotation
sf_controlpanel:
    resource: '@NewageerpSfControlpanelBundle/Controller'
    type:     annotation
sf_currency:
    resource: '@NewageerpSfCurrencyBundle/Controller'
    type:     annotation
sf_event-listener:
    resource: '@NewageerpSfEventListenerBundle/Controller'
    type:     annotation
sf_export:
    resource: '@NewageerpSfExportBundle/Controller'
    type:     annotation
sf_files:
    resource: '@NewageerpSfFilesBundle/Controller'
    type:     annotation
sf_follow-up:
    resource: '@NewageerpSfFollowUpBundle/Controller'
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
sf_status:
    resource: '@NewageerpSfStatusBundle/Controller'
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