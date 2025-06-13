```mermaid

sequenceDiagram
    title Dosen dan Tendik Menghapus Draft Surat di Politala Mail

    actor Dosen dan Tendik
    participant FilamentUI as Politala Mail UI
    participant MailResource
    participant MailModel as Mail
    participant DB as Database

    Dosen dan Tendik ->> FilamentUI: Klik "Hapus" pada Draft
    activate FilamentUI
    FilamentUI ->> MailResource: destroy($id)
    activate MailResource
    MailResource ->> MailModel: find draft
    activate MailModel
    MailModel ->> DB: SELECT * FROM mails WHERE id = ? AND released = false
    activate DB
    DB -->> MailModel: Draft ditemukan
    deactivate DB
    MailModel ->> DB: DELETE FROM mails WHERE id = ?
    activate DB
    DB -->> MailModel: Sukses
    deactivate DB
    deactivate MailModel
    MailResource -->> FilamentUI: Refresh Draft
    deactivate MailResource
    FilamentUI -->> Dosen dan Tendik: Draft berhasil dihapus
    deactivate FilamentUI


```