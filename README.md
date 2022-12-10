# Xdrabbit

Following blog:
https://blog.logrocket.com/react-native-form-validations-with-formik-and-yup/

Error fix following:----

https://stackoverflow.com/questions/71702392/viewproptypes-will-be-removed-from-react-native-migrate-to-viewproptypes-export

           --->
            1.Install patch-package into your project, as per the instructions.

            2.Install deprecated-react-native-prop-types by running npm install deprecated-react-native-prop-types or yarn add deprecated-react-native-prop-types.

            3.The invariant seems to be enforced in node_modules/react-native/index.js, starting at line 436:

                    get ColorPropType(): $FlowFixMe {
                        return require('deprecated-react-native-prop-types').ColorPropType
                    },
                    get EdgeInsetsPropType(): $FlowFixMe {
                        return require('deprecated-react-native-prop-types').EdgeInsetsPropType
                    },
                    get PointPropType(): $FlowFixMe {
                        return require('deprecated-react-native-prop-types').PointPropType
                    },
                    get ViewPropTypes(): $FlowFixMe {
                        return require('deprecated-react-native-prop-types').ViewPropTypes
                    },
                    };

            4.Save and run npx patch-package react-native to save the patch.

            5.Rebuild and the app should launch.

https://stackoverflow.com/questions/29133874/android-youtube-api-an-error-occurred-while-initializing-youtube-player

        --->
        1.Add the below lines of code into your AndroidManifest.xml file

        <queries>
        <intent>
            <action android:name="com.google.android.youtube.api.service.START" />
        </intent>
        </queries>
# Xdrabbit_RN
# xdrabbit-test
