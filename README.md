pwd
git status --short
git remote -v
      - name: Upload launcher APK
        uses: actions/upload-artifact@v4
        with:
          name: cleanyourtv-launcher
          path: launcher/app/build/outputs/apk/release/app-release.apk
          if-no-files-found: error
          retention-days: 7
          


