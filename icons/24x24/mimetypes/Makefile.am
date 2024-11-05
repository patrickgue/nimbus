size = 24x24
context = mimetypes
iconsdir = $(themedir)/$(size)/$(context)
icons_DATA = 				 		\
		gnome-fs-regular.icon 		\
		gnome-mime-application-x-backup.png 		\
		gnome-mime-application-x-core.png 		\
		gnome-mime-x-directory-nfs-server.png 		\
		gnome-mime-x-directory-nfs-share.png 		\
		gnome-mime-x-directory-smb-server.png 		\
		gnome-mime-x-directory-smb-share.png 		\
		stock_generic-mimetype.png \
		libreoffice-drawing.png \
		libreoffice-drawing-template.png \
		libreoffice-oasis-drawing.png \
		libreoffice-oasis-drawing-template.png \
		libreoffice-oasis-master-document.png \
		libreoffice-oasis-presentation.png \
		libreoffice-oasis-presentation-template.png \
		libreoffice-oasis-spreadsheet.png \
		libreoffice-oasis-spreadsheet-template.png \
		libreoffice-oasis-text.png \
		libreoffice-oasis-text-template.png \
		libreoffice-oasis-web-template.png \
		libreoffice-presentation.png \
		libreoffice-presentation-template.png \
		libreoffice-spreadsheet.png \
		libreoffice-spreadsheet-template.png \
		libreoffice-text.png \
		libreoffice-text-template.png \

EXTRA_DIST = $(icons_DATA)

install-data-local: install-iconsDATA
	(cd $(DESTDIR)$(themedir)/$(size) && $(ICONMAP) -c $(context) -e $(iconsrcdir)/icons/my-mapping.xml)

uninstall-local:
	rm -Rf $(DESTDIR)$(themedir)/$(size)/$(context)
